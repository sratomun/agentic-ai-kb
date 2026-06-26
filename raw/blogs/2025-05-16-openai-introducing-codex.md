# Introducing Codex

Source: https://openai.com/index/introducing-codex/
Author: OpenAI
Date: May 16, 2025 (with inline update June 3, 2025)
Category: Release / Product
Captured: 2026-06-22
Vendor stake: OpenAI launching/marketing its own coding agent (Codex / codex-1). SWE-Bench framing and customer quotes are self-reported.

---

A cloud-based software engineering agent that can work on many tasks in parallel, powered by codex-1. Available to ChatGPT Pro, Business, and Enterprise users today, and Plus users soon.

Codex performs tasks such as writing features, answering codebase questions, fixing bugs, and proposing pull requests. Each task runs in its own cloud sandbox environment, preloaded with your repository.

## codex-1
"Codex is powered by codex-1, a version of OpenAI o3 optimized for software engineering." Trained via reinforcement learning on real-world coding tasks to mirror human style and PR preferences, follow instructions, and iteratively run tests until passing.

- Task completion typically takes between 1 and 30 minutes; progress can be monitored in real time.
- Codex can read/edit files and run commands (test harnesses, linters, type checkers); commits changes in its environment.
- "Codex provides verifiable evidence of its actions through citations of terminal logs and test outputs, allowing you to trace each step taken during task completion."
- "Codex can be guided by AGENTS.md files placed within your repository."
- Benchmark conditions (footnote): "codex-1 was tested at a maximum context length of 192k tokens and medium 'reasoning effort,'..." and "23 SWE-Bench Verified samples that were not runnable on our internal infrastructure were excluded." (Headline SWE-Bench Verified numeric scores appear in chart images not captured as text.)

## Safety / guardrails
Users verify outputs through citations, terminal logs and test results; Codex explicitly communicates uncertainty and test failures. "Codex was trained to identify and precisely refuse requests aimed at development of malicious software, while clearly distinguishing and supporting legitimate tasks." OpenAI published an addendum to the o3 System Card. For secure execution, "during task execution, internet access is disabled... The agent cannot access external websites, APIs, or other services" (limited to provided GitHub repos and pre-installed dependencies).

## codex-mini
Also released: codex-mini, a version of o4-mini designed for Codex CLI, available as the default model in Codex CLI and in the API as `codex-mini-latest`. Priced at $1.50 per 1M input tokens and $6 per 1M output tokens, with a 75% prompt caching discount. Plus/Pro users signing into Codex CLI with ChatGPT could redeem $5 and $50 in free API credits respectively.

## Partners / usage
Early design partner Cisco; early testers Temporal, Superhuman, Kodiak (autonomous driving / Kodiak Driver). OpenAI engineers use Codex internally for refactoring, renaming, writing tests, and on-call triage.

June 3, 2025 update: Codex became available to Plus users and gained optional internet access during task execution.

Tags: Release · Product · Codex · 2025
