---
type: source
source_type: arxiv
title: "MemGraphRAG: Memory-based Multi-Agent System for Graph Retrieval-Augmented Generation"
authors: Chuanjie Wu, Zhishang Xiang, Yunbo Tang, Zerui Chen et al.
url: https://arxiv.org/abs/2606.00610v1
date: 2026-05-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.IR
tags: [knowledge-graph, agentic-rag, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MemGraphRAG: Memory-based Multi-Agent System for Graph Retrieval-Augmented Generation

**arXiv:** [2606.00610v1](https://arxiv.org/abs/2606.00610v1) · 2026-05-30 · cs.IR
**Authors:** Chuanjie Wu, Zhishang Xiang, Yunbo Tang, Zerui Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) has become an essential method for mitigating hallucinations in Large Language Models (LLMs) by leveraging external knowledge. Although effective for simple queries, traditional RAG struggles with large-scale, unstructured corpora where information is highly fragmented. Graph-based RAG (GraphRAG) incorporates knowledge graphs to capture structural relationships, enabling more comprehensive retrieval for complex reasoning. However, existing GraphRAG methods rely on isolated, fragment-level extraction for graph construction, lacking a global perspective on the whole corpus. As a result, these methods frequently lead to thematically inconsistent, logically conflicting, and structurally fragmented graphs that degrade retrieval performance. In this paper, we propose MemGraphRAG, a novel framework that introduces a memory-based multi-agent system to ensure high-quality graph construction. Specifically, MemGraphRAG employs a collaborative society of agents supported by shared memory, which provides a unified global context throughout the extraction process. This mechanism allows agents to dynamically resolve logical conflicts and maintain structural connectivity throughout the corpus. Furthermore, we propose a memory-aware hierarchical retrieval algorithm tailored for the constructed graph. Extensive experiments on multiple benchmarks demonstrate that MemGraphRAG outperforms the state-of-the-art baseline models with comparable efficiency. Our code is available at https://github.com/XMUDeepLIT/MemGraphRAG.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.00610v1)
