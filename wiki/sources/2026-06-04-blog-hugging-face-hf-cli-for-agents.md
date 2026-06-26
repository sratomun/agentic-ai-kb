---
type: source
source_type: blog
title: "Designing the hf CLI as an agent-optimized way to work with the Hub"
author: Célina Hanouti & Lucain Pouget (Hugging Face)
outlet: Hugging Face blog
url: https://huggingface.co/blog/hf-cli-for-agents
resource: https://huggingface.co/blog/hf-cli-for-agents
date: 2026-06-04
stake: HF is optimizing its own CLI to keep coding agents (and their traffic) flowing through the HF Hub; the benchmark is HF measuring its own tool, and the conclusion conveniently recommends adopting HF's CLI + skill.
ingested: 2026-06-22
tags: [perspective, coding-agents, tool-use, agent-skills, agent-evaluation]
---

# Designing the hf CLI as an agent-optimized way to work with the Hub

**Blog** · Célina Hanouti & Lucain Pouget (Hugging Face) · 2026-06-04 · [link](https://huggingface.co/blog/hf-cli-for-agents)

**The take (attributed):** HF argues that coding agents are now first-class *users* of developer tools, so a CLI should auto-detect when an agent (not a human) is driving and render differently — and that a well-designed CLI beats hand-rolled `curl`/SDK calls, using up to **6x fewer tokens** on multi-step tasks.

**Stake:** HF benchmarking HF's own `hf` CLI and recommending you install it + its skill. The token/success numbers are theirs; the design lessons generalize beyond HF.

## Argument
HF rebuilt `hf` to serve humans and agents from one command surface. Agents are detected via env vars they set (`CLAUDECODE`/`CLAUDE_CODE`, `CODEX_SANDBOX`, Cursor, Gemini, Pi, universal `AI_AGENT`), which both reshapes output and tags Hub traffic. By distinct users, **Claude Code (~39.5k users, ~48.6M requests) and Codex (~34.8k, ~36.4M)** dominate Hub agent traffic, ahead of antigravity, cursor, openclaw, gemini, pi.

Design principles for "agent-mode" output:
- **One command, two renderings:** humans get aligned/truncated tables with color; agents get full-fidelity TSV — no ANSI, nothing truncated, light on tokens.
- **Next-command hints** pre-filled with the IDs just used (a "rail" for the agent), errors that name the fix, hints to stderr so they don't pollute parsed stdout.
- **Non-blocking, safe-to-retry:** never waits on an interactive prompt; fails fast with `--yes`; idempotent ops (`--exist-ok`); `--dry-run` previews transfers.
- **Discoverable resource+verb tree** with copy-pasteable `--help` examples.

**The benchmark** (the durable part): 18 non-trivial Hub tasks, each via `hf` CLI vs curl/SDK, 10 reps, ~1,000 runs, graded by re-querying the live Hub (not trusting the agent's self-report), on Claude Code (Sonnet 4.6) and Codex (GPT-5.5). The CLI wins: success 0.94 vs 0.84 (Sonnet), 0.93 vs 0.92 (Codex); curl/SDK burn 1.3–1.8x tokens overall and **2.4x–6x on multi-step tasks** (bucket sync 6.0x, repo+branch+tag 2.4x) while near-parity on one-shot reads. Self-reported errors (agent claims success, Hub disagrees) far higher for curl/SDK. The **hf-cli skill** (auto-generated command reference) cuts tool calls ~30% (10.4→6.9 commands/run on Sonnet) without lowering the token bill.

## Why it matters / where it cuts
A rare *measured* look at how agents actually consume tools — and a concrete design pattern: agent-aware output, next-step rails, idempotent + non-blocking commands, and a [[agent-skills|skill]] as a command-surface cheat-sheet. It also quietly confirms Claude Code and Codex as the dominant [[coding-agents]] in the wild (by Hub traffic). So what: the transferable lesson is that tool ergonomics (token-efficiency, retry-safety, hints) measurably change agent success — relevant to any internal tooling he wants agents to drive. Discount that the winning tool is HF's own.

## Graph
- **Author:** [[hugging-face]]
- **Concepts:** [[coding-agents]] · [[tool-use]] · [[agent-skills]] · [[agent-evaluation]]
- **Entities:** [[hugging-face]] · [[claude]] · [[gpt-5]]
- **Raw:** `raw/blogs/2026-06-04-hugging-face-hf-cli-for-agents.md`
