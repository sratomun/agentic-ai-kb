---
type: source
source_type: arxiv
title: "SAG: SQL-Retrieval Augmented Generation with Query-Time Dynamic Hyperedges"
authors: Yuchao Wu, Junqin Li, XingCheng Liang, Yongjie Chen et al.
url: https://arxiv.org/abs/2606.15971v1
date: 2026-06-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.CL
tags: [knowledge-graph, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# SAG: SQL-Retrieval Augmented Generation with Query-Time Dynamic Hyperedges

**arXiv:** [2606.15971v1](https://arxiv.org/abs/2606.15971v1) · 2026-06-14 · cs.CL
**Authors:** Yuchao Wu, Junqin Li, XingCheng Liang, Yongjie Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) offers an effective approach for large language models to access external knowledge. However, existing methods rely on dense similarity retrieval and face inherent limitations in handling structured constraints and multi-hop reasoning. Incorporating knowledge graphs partially alleviates these issues, but at the cost of semantic fragmentation, high maintenance overhead, and difficult incremental updates. This paper introduces SAG (SQLRetrieval Augmented Generation), a structured architecture for retrieval and agent systems. Instead of pre-building a global static graph, SAG converts each chunk into one semantically complete event and a set of indexing entities, then uses SQL join queries to dynamically link events that share entities into local hyperedges,constructing, at query time, a dynamically instantiated local index structure. This design avoids the need for global graph rebuilding and ongoing maintenance; the system naturally supports incremental writes, concurrent processing, and continuous scaling through its reliance on standard database infrastructure. Across HotpotQA, 2WikiMultiHop, and MuSiQue, three standard multi-hop benchmarks,SAG achieves the best results on 8 out of 9 Recall@K metrics, reaching 80.0% Recall@5 on MuSiQue, the benchmark with the highest multi-hop reasoning demands.SAG has also been deployed at a production scale of hundreds of millions of data items, with online retrieval latency kept within seconds. Project site and code are available at https://github.com/Zleap-AI/SAG-Benchmark.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.15971v1)
