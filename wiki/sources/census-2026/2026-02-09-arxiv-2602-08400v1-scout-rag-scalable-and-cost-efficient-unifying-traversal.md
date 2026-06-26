---
type: source
source_type: arxiv
title: "SCOUT-RAG: Scalable and Cost-Efficient Unifying Traversal for Agentic Graph-RAG over Distributed Domains"
authors: Longkun Li, Yuanben Zou, Jinghan Wu, Yuqing Wen et al.
url: https://arxiv.org/abs/2602.08400v1
date: 2026-02-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, agentic-rag, arxiv, auto-ingested]
---

# SCOUT-RAG: Scalable and Cost-Efficient Unifying Traversal for Agentic Graph-RAG over Distributed Domains

**arXiv:** [2602.08400v1](https://arxiv.org/abs/2602.08400v1) · 2026-02-09 · cs.AI
**Authors:** Longkun Li, Yuanben Zou, Jinghan Wu, Yuqing Wen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph-RAG improves LLM reasoning using structured knowledge, yet conventional designs rely on a centralized knowledge graph. In distributed and access-restricted settings (e.g., hospitals or multinational organizations), retrieval must select relevant domains and appropriate traversal depth without global graph visibility or exhaustive querying. To address this challenge, we introduce \textbf{SCOUT-RAG} (\textit{\underline{S}calable and \underline{CO}st-efficient \underline{U}nifying \underline{T}raversal}), a distributed agentic Graph-RAG framework that performs progressive cross-domain retrieval guided by incremental utility goals. SCOUT-RAG employs four cooperative agents that: (i) estimate domain relevance, (ii) decide when to expand retrieval to additional domains, (iii) adapt traversal depth to avoid unnecessary graph exploration, and (iv) synthesize the high-quality answers. The framework is designed to minimize retrieval regret, defined as missing useful domain information, while controlling latency and API cost. Across multi-domain knowledge settings, SCOUT-RAG achieves performance comparable to centralized baselines, including DRIFT and exhaustive domain traversal, while substantially reducing cross-domain calls, total tokens processed, and latency.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.08400v1)
