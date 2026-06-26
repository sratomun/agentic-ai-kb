# Designing the hf CLI as an agent-optimized way to work with the Hub

Source: https://huggingface.co/blog/hf-cli-for-agents
Authors: Célina Hanouti, Lucain Pouget
Date: June 4, 2026
Outlet: Hugging Face blog
Captured: 2026-06-22

---

`hf` is the official command-line entrypoint to the Hugging Face Hub. Anything you can do on the Hub from the Python SDK, you can do from your terminal: download and upload models, datasets and Spaces; create and manage repos, branches, tags and pull requests; run Jobs on HF infrastructure; manage Buckets, Collections, webhooks and Inference Endpoints.

The `hf` CLI has been primarily built for our users over the years. But it's now increasingly used by **coding agents**: Claude Code, Codex, Cursor and more. So we rebuilt it to make it work for both audiences at once. We found that on complex, multi-step tasks the no-CLI baseline (an agent hand-rolling `curl` or the Python SDK) uses up to **6x as many tokens** as the `hf` CLI.

## AI agent traffic on the Hub

We started tracking agent usage of the Hub in April 2026. The CLI detects when a coding agent is driving it by reading the environment variables agents set: `CLAUDECODE`/`CLAUDE_CODE` for Claude Code, `CODEX_SANDBOX` for Codex, plus Cursor, Gemini, Pi, and the universal `AI_AGENT`. That signal shapes the CLI's output and tags each Hub request with an `agent/<name>` user-agent.

The two largest by distinct users are **Claude Code and Codex**, well ahead of everything else. Claude Code leads with ~39.5k users and ~48.6M requests, then Codex with ~34.8k users and ~36.4M requests, followed by antigravity, cursor-cli, openclaw, cursor, gemini and pi.

## Built for humans and agents

Humans want rich terminal output (ANSI color, padded tables, progress bars). An agent wants the inverse: no ANSI, nothing truncated, every value in full, kept compact and structured to stay light on tokens. Agent-mode output was introduced in `hf` v1.9.0.

- **One command, multiple renderings.** When `hf` auto-detects agent use, it renders the same command differently — a human gets an aligned table truncated to fit; an agent gets the complete record as TSV (full ids, ISO timestamps, every tag, no ANSI, nothing truncated). `--json`/`--quiet` options also available; users can force `--format human | agent | json | quiet`.
- **Next-command hints.** Many `hf` commands end with a hint: the exact next command to run, pre-filled with the IDs you just used. Errors name the fix (`Run hf auth login first.`). Hints/warnings/errors go to stderr while data goes to stdout.
- **Non-blocking and safe to retry.** `hf` never sits on an interactive prompt. A destructive command fails fast with the fix in the message (`Use --yes to skip confirmation.`). Operations are safe to repeat (`--exist-ok`, idempotent re-uploads). `--dry-run` previews data transfers.
- **Discoverable, predictable commands.** Consistent resource + verb tree (`hf models ls`, `hf repos create`, `hf jobs ps`) with aliases. Every `--help` ends with copy-pasteable examples. `-q` prints one id per line; `--json` pipes to `jq`.

## Benchmarking the hf CLI for Coding Agents

18 non-trivial Hub tasks (aggregate a trending org's models, upload with include/exclude rules, copy files across repos, open a PR adding a license, create a repo with a branch and tag, sync and prune a bucket, build a collection). Each task goes to a fresh agent with exactly one way to talk to the Hub: the `hf` CLI, or curl/the Python SDK. Each combination run 10 times; ~1,000 graded runs total. Runs graded independently by re-querying the live Hub (not trusting the agent's self-report). Ran on Claude Code (Sonnet 4.6) and OpenAI Codex (GPT-5.5).

Results table:

| agent | tool | success score | token usage | self-report error |
| --- | --- | --- | --- | --- |
| Claude Code (Sonnet 4.6) | hf CLI | 0.94 | baseline | 2 / 163 |
|  | curl / Python SDK | 0.84 | 1.3-1.6x tokens | 11 / 163 |
| Codex (GPT-5.5) | hf CLI | 0.93 | baseline | 3 / 163 |
|  | curl / Python SDK | 0.92 | 1.6-1.8x tokens | 10 / 163 |

### Key findings

- The `hf` CLI is far leaner than curl or the SDK. For the same task, at equal-or-better success, curl and the SDK burn roughly 1.3x to 1.8x the tokens. On easy reads they're fine, but on real multi-step work they pay 2x to 6x: the CLI composes a chain of REST calls into a few high-level commands. (Per-task token ratios: bucket create+sync+prune 6.0x, rank orgs by trending models 4.1x, repo create+branch+tag / delete files / copy files across repos 2.4x each; simple reads near parity or cheaper — batch metadata 0.5x, count rows 0.3x.)
- On a stronger model (GPT-5.5) curl and the SDK work but stay wasteful; on Sonnet they can't finish parts of the job (the writes, mostly).

## The hf-cli skill

`hf` ships a skill: a compact, auto-generated reference of the whole command surface that an agent loads as context. With the skill, mean commands per run drop from ~10.4 to 6.9 (Sonnet) and ~10.1 to 7.3 (Codex) — roughly 30% fewer tool calls. The skill doesn't cut the token bill (fixed context cost) or make the CLI more reliable, but the agent spends time running the task rather than finding out how the tool works. `hf skills add` / `hf skills add --claude`.

## Register an agent harness

Building an agent harness? Get it registered via a PR to `agent-harnesses.ts` so `hf` learns to detect it and the Hub attributes its traffic.
