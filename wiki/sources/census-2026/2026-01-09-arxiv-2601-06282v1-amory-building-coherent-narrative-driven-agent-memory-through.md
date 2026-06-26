---
type: source
source_type: arxiv
title: "Amory: Building Coherent Narrative-Driven Agent Memory through Agentic Reasoning"
authors: Yue Zhou, Xiaobo Guo, Belhassen Bayar, Srinivasan H. Sengamedu
url: https://arxiv.org/abs/2601.06282v1
date: 2026-01-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CL
tags: [agentic-rag, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Amory: Building Coherent Narrative-Driven Agent Memory through Agentic Reasoning

**arXiv:** [2601.06282v1](https://arxiv.org/abs/2601.06282v1) · 2026-01-09 · cs.CL
**Authors:** Yue Zhou, Xiaobo Guo, Belhassen Bayar, Srinivasan H. Sengamedu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-term conversational agents face a fundamental scalability challenge as interactions extend over time: repeatedly processing entire conversation histories becomes computationally prohibitive. Current approaches attempt to solve this through memory frameworks that predominantly fragment conversations into isolated embeddings or graph representations and retrieve relevant ones in a RAG style. While computationally efficient, these methods often treat memory formation minimally and fail to capture the subtlety and coherence of human memory. We introduce Amory, a working memory framework that actively constructs structured memory representations through enhancing agentic reasoning during offline time. Amory organizes conversational fragments into episodic narratives, consolidates memories with momentum, and semanticizes peripheral facts into semantic memory. At retrieval time, the system employs coherence-driven reasoning over narrative structures. Evaluated on the LOCOMO benchmark for long-term reasoning, Amory achieves considerable improvements over previous state-of-the-art, with performance comparable to full context reasoning while reducing response time by 50%. Analysis shows that momentum-aware consolidation significantly enhances response quality, while coherence-driven retrieval provides superior memory coverage compared to embedding-based approaches.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.06282v1)
