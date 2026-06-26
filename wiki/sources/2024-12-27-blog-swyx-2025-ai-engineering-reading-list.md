---
type: source
source_type: blog
title: "The 2025 AI Engineering Reading List"
author: swyx (Shawn Wang)
outlet: Latent.Space
url: https://www.latent.space/p/2025-papers
resource: https://www.latent.space/p/2025-papers
date: 2024-12-27
stake: Founder/CEO of AI Engineer + Latent Space — the canonical "what an AI Engineer should read" list, which reinforces his framing of the discipline (and is partly paywalled, a Substack product).
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-evaluation, agent-memory, tool-use, coding-agents]
---

# The 2025 AI Engineering Reading List

**Blog** · swyx (Shawn Wang) · 2024-12-27 (continuously maintained) · [link](https://www.latent.space/p/2025-papers)

**The take (attributed):** swyx curates "50 papers/models/blogs across 10 fields" as the *practical* canon for an AI Engineer — explicitly skipping foundational ML theory ("no time wasted on Attention is All You Need") in favor of what you actually need at work.

**Stake:** This is the de facto AI Engineer syllabus, which entrenches his definition of the discipline; partly paywalled (a Substack product).

## Argument (Agents section, the agent-relevant core)
swyx's five required agent reads, each with a "why it matters":
1. **[[swe-bench|SWE-Bench]]** (& SWE-Lancer) — "probably the highest profile agent benchmark today"; "technically a coding benchmark, but more a test of agents than raw LLMs." Plus [[tau-bench|TauBench]] and [[gaia-benchmark|GAIA]] for tool-agent-user interaction.
2. **[[react|ReAct]]** — "started a long line of research on tool using and function calling LLMs" ([[tool-use]]).
3. **MemGPT** — "one of many notable approaches to emulating long running agent memory" ([[agent-memory]]), adopted by ChatGPT and [[langgraph|LangGraph]].
4. **Voyager** — Nvidia's curriculum / skill library / sandbox cognitive architecture; skill libraries as a form of agent memory.
5. **Anthropic's Building Effective Agents** — "a great state-of-2024 recap" on chaining, routing, parallelization, orchestration, evaluation, optimization.

Broader framing he asserts: reasoning models dominate the 2025 frontier; **benchmarks saturate increasingly quickly** and "the whole approach is getting dated, new approaches are needed" ([[agent-evaluation]]); China open models (Kimi K-2, Qwen 3) have overtaken; much of the agent/codegen frontier "has moved from research to industry" and lives in blogposts/talks, not papers.

## Why it matters / where it cuts
The single most-shared "where to start" map for the field, so it shapes what a generation of AI Engineers consider canonical — useful to the radar as a cross-check on which benchmarks/methods the practitioner consensus actually weights ([[swe-bench]], [[react]], [[tau-bench]] over flashier alternatives). His "benchmarks are getting dated" line is the opinion-layer echo of the radar's own [[agent-evaluation]] concerns.

## Graph
- **Author:** [[swyx]]
- **Concepts:** [[agentic-ai]] · [[agent-evaluation]] · [[agent-memory]] · [[tool-use]] · [[coding-agents]]
- **Entities:** [[swe-bench]] · [[tau-bench]] · [[gaia-benchmark]] · [[react]] · [[langgraph]] · [[anthropic]]
- **Raw:** `raw/blogs/2024-12-27-swyx-2025-ai-engineering-reading-list.md`
