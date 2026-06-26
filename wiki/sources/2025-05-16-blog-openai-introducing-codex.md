---
type: source
source_type: blog
title: "Introducing Codex"
author: OpenAI
outlet: OpenAI news
url: https://openai.com/index/introducing-codex/
resource: https://openai.com/index/introducing-codex/
date: 2025-05-16
stake: Vendor product launch — OpenAI shipping and marketing Codex (cloud coding agent, codex-1) and codex-mini. SWE-Bench framing, customer quotes (Cisco, Temporal, Superhuman, Kodiak), and "malicious-software refusal" claims are OpenAI's own.
ingested: 2026-06-22
tags: [perspective, agentic-ai, coding-agents, tool-use, reasoning-models, agent-security]
---

# Introducing Codex

**Blog** · OpenAI · 2025-05-16 · [link](https://openai.com/index/introducing-codex/)

**The take (attributed):** OpenAI argues software engineering is the first place autonomous agents pay off, and ships Codex as a cloud-based [[coding-agents|coding agent]] — a [[reasoning-models|reasoning model]] (codex-1, a version of [[openai-o3|o3]]) fine-tuned by RL to work in its own sandbox, run tests until they pass, and produce verifiable PRs with cited terminal logs.

**Stake:** Product launch. The SWE-Bench-Verified framing and customer logos are OpenAI marketing its own coding agent. The genuinely notable, checkable bits are architectural: a per-task isolated sandbox, **no internet during execution**, `AGENTS.md` steering, and citation-backed terminal logs.

## Argument
Codex runs many tasks in parallel, each in its own cloud sandbox preloaded with your repo — writing features, fixing bugs, answering codebase questions, proposing PRs. It's powered by **codex-1**, "a version of OpenAI o3 optimized for software engineering," trained via [[agentic-rl|reinforcement learning]] on real coding tasks to mirror human PR style and iterate on tests until passing.
- Tasks "typically take between 1 and 30 minutes," monitorable in real time.
- It runs commands (test harnesses, linters, type checkers), commits in its environment, and "provides verifiable evidence of its actions through citations of terminal logs and test outputs."
- Steerable via **`AGENTS.md`** files in the repo ([[agent-skills|agent instructions/skills]] pattern).
- Benchmark caveats (footnote): tested at 192k-token max context, medium "reasoning effort"; 23 [[swe-bench|SWE-Bench Verified]] samples excluded as non-runnable on internal infra. (Headline SWE-Bench scores live in chart images not in the captured text.)

On [[agent-security|safety]]: outputs verifiable via citations/logs/tests; Codex "explicitly communicates" uncertainty and test failures; trained to "identify and precisely refuse requests aimed at development of malicious software." For secure execution, "internet access is disabled" during task execution — the agent can't reach external sites/APIs, only the provided repo and pre-installed deps. Also shipped **codex-mini** (a version of o4-mini for Codex CLI; `codex-mini-latest` at $1.50/$6 per 1M tokens, 75% cache discount). Early partners: Cisco, Temporal, Superhuman, Kodiak.

## Why it matters / where it cuts
Codex is OpenAI's entry in the [[coding-agents|cloud coding-agent]] race and the seed of what became its biggest agent franchise (by 2026 the OpenAI blog is dominated by Codex enterprise case studies and Codex-for-knowledge-work). So what: the architecture is the lesson, not the benchmark — **sandbox-per-task + no-internet-during-execution + cited test logs** is the reliability-and-trust pattern serious coding agents converge on, and `AGENTS.md` is the now-standard repo-level steering file. The "refuse malicious software" training is an early example of safety-for-coding-agents that later expands into OpenAI's whole Codex-Security/cyber-defense line. Treat the SWE-Bench framing as vendor; treat the sandbox-isolation design as the durable signal.

## Graph
- **Author:** [[openai]]
- **Concepts:** [[coding-agents]] · [[agentic-ai]] · [[tool-use]] · [[reasoning-models]] · [[agentic-rl]] · [[agent-skills]] · [[agent-security]]
- **Entities:** [[openai]] · [[openai-o3]] · [[swe-bench]]
- **Raw:** `raw/blogs/2025-05-16-openai-introducing-codex.md`
