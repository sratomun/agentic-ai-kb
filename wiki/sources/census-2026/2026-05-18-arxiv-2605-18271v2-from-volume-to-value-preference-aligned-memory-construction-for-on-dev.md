---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "From Volume to Value: Preference-Aligned Memory Construction for On-Device RAG"
authors: Changmin Lee et al.
url: https://arxiv.org/abs/2605.18271v2
date: 2026-05-18
score: 1
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, agentic-rag, recommendation-agents]
---

# From Volume to Value: Preference-Aligned Memory Construction for On-Device RAG

**arXiv:** [2605.18271v2](https://arxiv.org/abs/2605.18271v2) · 2026-05-18 · cs.CL
**Authors:** Changmin Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
With the rapid emergence of personal AI agents based on Large Language Models (LLMs), implementing them on-device has become essential for privacy and responsiveness. To handle the inherently personal and context-dependent nature of real-world requests, such agents must ground their generation in device-resident personal context. However, under tight memory budgets, the core bottleneck is what to store so that retrieval remains aligned with the user. We propose EPIC (Efficient Preference-aligned Index Construction), which focuses on user preferences as a compact and stable form of personal context and integrates them throughout the RAG pipeline. EPIC selectively retains preference-relevant information from raw data and aligns retrieval toward preference-aligned contexts. Across four benchmarks covering conversations, debates, explanations, and recommendations, EPIC reduces indexing memory by 2,404 times, improves preference-following accuracy by 18.79 %p, and achieves 32.17 times lower retrieval latency over the best-performing baseline. In on-device experiments, EPIC maintains under 1 MB memory and achieves 5.21 to 29.35 ms/query latency across three platforms, while supporting streaming updates under preference drift. Our code and data are available at https://github.com/UbiquitousAILab/EPIC.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[agentic-rag]] · [[recommendation-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.18271v2)
