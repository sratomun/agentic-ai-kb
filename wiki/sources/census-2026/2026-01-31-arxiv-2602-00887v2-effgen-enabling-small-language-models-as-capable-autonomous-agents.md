---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "EffGen: Enabling Small Language Models as Capable Autonomous Agents"
authors: Gaurav Srivastava et al.
url: https://arxiv.org/abs/2602.00887v2
date: 2026-01-31
score: 16
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, agent-memory, llm-as-judge]
---

# EffGen: Enabling Small Language Models as Capable Autonomous Agents

**arXiv:** [2602.00887v2](https://arxiv.org/abs/2602.00887v2) · 2026-01-31 · cs.CL
**Authors:** Gaurav Srivastava et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Most existing language model agentic systems today are built and optimized for large language models (e.g., GPT, Claude, Gemini) via API calls; while powerful, this approach faces several limitations including high token costs and privacy concerns for sensitive applications. We introduce EffGen, an open-source agentic framework optimized for small language models (SLMs) that enables effective, efficient, and secure local deployment. EffGen makes four major contributions: (1) Enhanced tool-calling with prompt optimization that compresses input prompts by up to 70-80% (and 57% on average across our benchmarks) while preserving task semantics, (2) Intelligent task decomposition that breaks complex queries into parallel or sequential subtasks based on dependencies, (3) Complexity-based routing using five factors to make smart pre-execution decisions, and (4) Unified memory system combining short-term, long-term, and vector-based storage. Additionally, EffGen unifies multiple agent protocols (MCP, A2A, ACP) for cross-protocol communication. Results on 13 benchmarks show EffGen outperforms LangChain, AutoGen, and Smolagents with higher success rates, faster execution, and lower memory. Our results reveal that prompt optimization and complexity routing have complementary scaling behavior: optimization benefits SLMs more (11.2% gain at 1.5B vs 2.4% at 32B), while routing benefits large models more (3.6% at 1.5B vs 7.9% at 32B), providing consistent gains across all scales when combined. EffGen is released under the Apache 2.0 License, ensuring broad accessibility for research and commercial use, with the code available at https://github.com/ctrl-gaurav/effGen, the Python package at https://pypi.org/project/effgen/ (pip install effgen), and the project website and documentation at https://effgen.org/ and https://docs.effgen.org/.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[agent-memory]] · [[llm-as-judge]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.00887v2)
