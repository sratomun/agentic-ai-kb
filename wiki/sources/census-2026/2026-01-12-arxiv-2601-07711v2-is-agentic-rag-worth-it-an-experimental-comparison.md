---
type: source
source_type: arxiv
title: "Is Agentic RAG worth it? An experimental comparison of RAG approaches"
authors: Pietro Ferrazzi, Milica Cvjeticanin, Alessio Piraccini, Davide Giannuzzi
url: https://arxiv.org/abs/2601.07711v2
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# Is Agentic RAG worth it? An experimental comparison of RAG approaches

**arXiv:** [2601.07711v2](https://arxiv.org/abs/2601.07711v2) · 2026-01-12 · cs.CL
**Authors:** Pietro Ferrazzi, Milica Cvjeticanin, Alessio Piraccini, Davide Giannuzzi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) systems are usually defined by the combination of a generator and a retrieval component that extracts textual context from a knowledge base to answer user queries. However, such basic implementations exhibit several limitations, including noisy or suboptimal retrieval, misuse of retrieval for out-of-scope queries, weak query-document matching, and variability or cost associated with the generator. These shortcomings have motivated the development of "Enhanced" RAG, where dedicated modules are introduced to address specific weaknesses in the workflow. More recently, the growing self-reflective capabilities of Large Language Models (LLMs) have enabled a new paradigm, often referred to as "Agentic" RAG. In this approach, an LLM orchestrates the entire process, deciding which actions to perform, when to perform them, and whether to iterate. Despite the rapid adoption of both paradigms, it remains unclear which approach is preferable under which conditions. In this work, we conduct an empirically driven evaluation of "Enhanced" and "Agentic" RAG across multiple scenarios and dimensions. Our results provide practical insights into the trade-offs between the two paradigms, offering guidance on selecting the most effective RAG design for real-world applications, considering both performance and costs.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.07711v2)
