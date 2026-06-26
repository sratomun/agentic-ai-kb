---
type: source
source_type: arxiv
title: "HyperGraphPro: Progress-Aware Reinforcement Learning for Structure-Guided Hypergraph RAG"
authors: Jinyoung Park, Sanghyeok Lee, Omar Zia Khan, Hyunwoo J. Kim et al.
url: https://arxiv.org/abs/2601.17755v2
date: 2026-01-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.CL
tags: [knowledge-graph, agentic-rl, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# HyperGraphPro: Progress-Aware Reinforcement Learning for Structure-Guided Hypergraph RAG

**arXiv:** [2601.17755v2](https://arxiv.org/abs/2601.17755v2) · 2026-01-25 · cs.CL
**Authors:** Jinyoung Park, Sanghyeok Lee, Omar Zia Khan, Hyunwoo J. Kim et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph Retrieval-Augmented Generation (GraphRAG) has emerged as a promising paradigm that organizes external knowledge into structured graphs of entities and relations, enabling large language models (LLMs) to perform complex reasoning beyond text-chunk retrieval. Recent advances have integrated reinforcement learning (RL) into agentic GraphRAG approaches, enabling iterative interactions with knowledge graphs during training. However, existing RL-based methods suffer from two key limitations: (1) they primarily depend on semantic similarity for retrieval, often overlooking the underlying graph topology, and (2) they rely on sparse, outcome-level rewards that fail to capture the quality of intermediate retrieval steps and their dependencies. To address these limitations, we propose HyperGraphPro, a progress-aware agentic framework for graph-based retrieval and multi-step reasoning. HyperGraphPro introduces a structure-aware hypergraph retrieval mechanism that jointly considers semantic relevance and graph connectivity, promoting coherent traversal along multi-hop reasoning paths. Furthermore, we design a progress-based stepwise policy optimization that provides dense learning signals by modulating advantages according to intermediate reasoning progress within a graph, rather than relying solely on final outcomes. Experiments on multi-hop question answering benchmarks demonstrate that HyperGraphPro consistently improves reasoning accuracy and generation quality over existing GraphRAG methods.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.17755v2)
