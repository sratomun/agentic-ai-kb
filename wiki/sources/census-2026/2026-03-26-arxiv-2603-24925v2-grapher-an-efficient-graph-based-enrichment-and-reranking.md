---
type: source
source_type: arxiv
title: "GraphER: An Efficient Graph-Based Enrichment and Reranking Method for Retrieval-Augmented Generation"
authors: Ruizhong Miao, Yuying Wang, Rongguang Wang, Chenyang Li et al.
url: https://arxiv.org/abs/2603.24925v2
date: 2026-03-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.LG
tags: [knowledge-graph, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# GraphER: An Efficient Graph-Based Enrichment and Reranking Method for Retrieval-Augmented Generation

**arXiv:** [2603.24925v2](https://arxiv.org/abs/2603.24925v2) · 2026-03-26 · cs.LG
**Authors:** Ruizhong Miao, Yuying Wang, Rongguang Wang, Chenyang Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-augmented generation (RAG) systems that rely on semantic search often fail to retrieve the complete set of evidence for complex queries, particularly when information is distributed across multiple sources. Existing approaches either rely on iterative agentic retrieval, which can be inefficient, or maintain additional structures such as knowledge graphs, which introduce storage and maintenance overhead. In this paper, we propose GraphER, a graph-based enrichment and reranking framework that (1) leverages the organizational structure of data to capture proximity relationships beyond semantic similarity, (2) constructs a graph at query time based on these proximities, and (3) applies graph-based ranking to surface the top candidate documents. Experiments across table retrieval, multi-hop retrieval, and long-document retrieval benchmarks demonstrate consistent improvements in terms of retrieval completeness. Additionally, GraphER requires no additional graph infrastructure and integrates seamlessly with standard vector stores. The framework is retriever-agnostic, supports multiple forms of proximity, and introduces minimal query-time latency.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.24925v2)
