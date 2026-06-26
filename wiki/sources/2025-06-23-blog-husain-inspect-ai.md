---
type: source
source_type: blog
title: "Inspect AI, An OSS Python Library For LLM Evals"
author: Hamel Husain
outlet: hamel.dev
url: https://hamel.dev/notes/llm/evals/inspect.html
resource: https://hamel.dev/notes/llm/evals/inspect.html
date: 2025-06-23
stake: Independent ML consultant (Parlance Labs); JJ Allaire guest-lectured in Husain's paid evals course, and the post promotes that course (with a discount code) — but Inspect is third-party OSS Husain has no commercial stake in.
ingested: 2026-06-22
tags: [perspective, evaluation, agent-evaluation, llm-as-judge, agent-frameworks]
---

# Inspect AI, An OSS Python Library For LLM Evals

**Blog (annotated guest lecture)** · Hamel Husain (hamel.dev), presenting JJ Allaire · 2025-06-23 · [link](https://hamel.dev/notes/llm/evals/inspect.html)

**The take (attributed):** Husain spotlights **Inspect AI** — JJ Allaire's (RStudio/Posit founder) open-source eval framework, built at the UK AI Safety Institute and now the eval framework of choice at **Anthropic, DeepMind, and Grok** — as a production-grade, reproducible substrate for LLM and **agent** evaluation that bridges research and production.

**Stake:** Husain is presenting someone else's tool (no commercial stake in Inspect); the post does market his course. The endorsement carries weight precisely because Inspect is the frontier labs' choice, not a vendor pitch.

## Argument
An annotated walk-through of Allaire's lecture. Inspect's spine is three concepts: **Dataset** (input + target), **Solver** (a Python function transforming a `TaskState` — from a single model call to self-critique chains to full agent scaffolds with tool use), and **Scorer** (text match, model-graded/LLM-as-judge, or custom). It offers a high-level composable API and a low-level "deep universal LLM interface" (caching, logging, metrics, parallelism) for building advanced agents.

Agent-eval relevant features: first-class tool use (`use_tools()` + an auto-resolving generation/tool loop); **Agent Bridges** that monkey-patch the OpenAI client to evaluate *existing* LangChain/Autogen/Claude-Code agents without rewriting them; sub-agent `TaskState` forking; **sandbox environments** for untrusted code; an **interactive approval** system (human approves/rejects sensitive tool calls — a safety layer for agentic evals); and built-in agent benchmarks **GAIA, GDM Dangerous Capabilities (CTF), and SWE-Bench**. Production: parallelism, **Eval Sets** (auto-retry, resume, reuse failed samples), comprehensive structured `EvalLog` logging with a viewer (bootstrap std-dev, message/thinking history), and a VS Code plugin. Notably, Allaire insists Inspect's agent tools are **for evals only** — you should run the *same* pipeline for evals and production, not maintain separate tools. Q&A: jailbreaks bypass refusals but don't improve capability benchmarks; latency/token-cost tracking is built in.

## Why it matters / where it cuts
This is the radar's concrete answer to "what do serious labs actually use to evaluate agents." It grounds [[agent-evaluation]] in real tooling (GAIA/SWE-Bench/CTF harnesses, sandboxing, human approval) and models the [[llm-as-judge]] pattern as a pluggable, customizable scorer. Allaire's "same pipeline for evals and prod" principle echoes Husain's own evals-first discipline. So what: if a team is standardizing agent evals, Inspect (frontier-lab-adopted, OSS, AISI-built) is the default to evaluate — and the Agent Bridge means existing agents can be wrapped without a rewrite.

## Graph
- **Author:** [[hamel-husain]]
- **Concepts:** [[agent-evaluation]] · [[llm-as-judge]]
- **Entities:** [[inspect-ai]] (the framework — node requested) · [[anthropic]] · [[swe-bench]] · [[gaia-benchmark]]
- **Raw:** `raw/blogs/2025-06-23-husain-inspect-ai.md`
