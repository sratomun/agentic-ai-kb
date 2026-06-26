---
type: source
source_type: arxiv
title: "HyperMem: Hypergraph Memory for Long-Term Conversations"
authors: Juwei Yue, Chuanrui Hu, Jiawei Sheng, Zuyi Zhou et al.
url: https://arxiv.org/abs/2604.08256v2
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.CL
tags: [knowledge-graph, agentic-rag, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# HyperMem: Hypergraph Memory for Long-Term Conversations

**arXiv:** [2604.08256v2](https://arxiv.org/abs/2604.08256v2) · 2026-04-09 · cs.CL
**Authors:** Juwei Yue, Chuanrui Hu, Jiawei Sheng, Zuyi Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Long-term memory is essential for conversational agents to maintain coherence, track persistent tasks, and provide personalized interactions across extended dialogues. However, existing approaches as Retrieval-Augmented Generation (RAG) and graph-based memory mostly rely on pairwise relations, which can hardly capture high-order associations, i.e., joint dependencies among multiple elements, causing fragmented retrieval. To this end, we propose HyperMem, a hypergraph-based hierarchical memory architecture that explicitly models such associations using hyperedges. Particularly, HyperMem structures memory into three levels: topics, episodes, and facts, and groups related episodes and their facts via hyperedges, unifying scattered content into coherent units. Leveraging this structure, we design a hybrid lexical-semantic index and a coarse-to-fine retrieval strategy, supporting accurate and efficient retrieval of high-order associations. Experiments on the LoCoMo benchmark show that HyperMem achieves state-of-the-art performance with 92.73% LLM-as-a-judge accuracy, demonstrating the effectiveness of HyperMem for long-term conversations.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.08256v2)
