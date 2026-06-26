---
type: source
source_type: arxiv
title: "Mixture-of-Experts Knowledge Graph Retrieval-Augmented Generation for Multi-Agent LLM-based Recommendation"
authors: Shijie Wang, Chengyi Liu, Yujuan Ding, Shanru Lin et al.
url: https://arxiv.org/abs/2605.28175v2
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.IR
tags: [recommendation-agents, knowledge-graph, agentic-rl, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# Mixture-of-Experts Knowledge Graph Retrieval-Augmented Generation for Multi-Agent LLM-based Recommendation

**arXiv:** [2605.28175v2](https://arxiv.org/abs/2605.28175v2) · 2026-05-27 · cs.IR
**Authors:** Shijie Wang, Chengyi Liu, Yujuan Ding, Shanru Lin et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) have recently been adopted for recommendations due to their ability to understand user intent and item semantics. However, LLM-based recommender systems often rely on parametric knowledge and suffer from outdated knowledge, motivating knowledge graph retrieval-augmented generation (KG-RAG) to ground recommendations on structured, up-to-date KGs. Despite this promise, effective KG-RAG in recommendations faces great challenges. First, users' queries vary in complexity and require KG knowledge at different granularities, whereas existing methods adopt a one-size-fits-all retrieval strategy, leading to over-retrieval for simple queries and under-retrieval for complex ones. In addition, augmenting LLMs with KG knowledge requires translating graph-structured data into linear text, which may introduce noise and cause structural information loss. Moreover, the selection of retrieval granularity lacks direct supervision and must be inferred from the final recommendation after alignment and downstream utilization, making query-aware retrieval hard to learn end-to-end. To address these issues, we propose MixRAGRec, a cooperative multi-agent framework for KG-RAG recommendations. MixRAGRec integrates a Mixture-of-Experts Retrieval Agent that routes each query to a KG retrieval expert with different granularities, a Knowledge Preference Alignment Agent that converts structured knowledge into LLM-friendly natural language, and a Contrastive Learning-reinforced Recommendation Agent trained with contrastive preference feedback. Notably, we introduce Mixture-of-Experts Multi-Agent Policy Optimization (MMAPO) to train three agents under a unified objective. Extensive experiments on real-world datasets demonstrate the effectiveness of our framework.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28175v2)
