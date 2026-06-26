---
type: source
source_type: arxiv
title: "Pruning Minimal Reasoning Graphs for Efficient Retrieval-Augmented Generation"
authors: Ning Wang, Kuanyan Zhu, Daniel Yuehwoon Yee, Yitang Gao et al.
url: https://arxiv.org/abs/2602.04926v1
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.DB
tags: [clinical-agents, knowledge-graph, agentic-rag, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Pruning Minimal Reasoning Graphs for Efficient Retrieval-Augmented Generation

**arXiv:** [2602.04926v1](https://arxiv.org/abs/2602.04926v1) · 2026-02-04 · cs.DB
**Authors:** Ning Wang, Kuanyan Zhu, Daniel Yuehwoon Yee, Yitang Gao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-augmented generation (RAG) is now standard for knowledge-intensive LLM tasks, but most systems still treat every query as fresh, repeatedly re-retrieving long passages and re-reasoning from scratch, inflating tokens, latency, and cost. We present AutoPrunedRetriever, a graph-style RAG system that persists the minimal reasoning subgraph built for earlier questions and incrementally extends it for later ones. AutoPrunedRetriever stores entities and relations in a compact, ID-indexed codebook and represents questions, facts, and answers as edge sequences, enabling retrieval and prompting over symbolic structure instead of raw text. To keep the graph compact, we apply a two-layer consolidation policy (fast ANN/KNN alias detection plus selective $k$-means once a memory threshold is reached) and prune low-value structure, while prompts retain only overlap representatives and genuinely new evidence. We instantiate two front ends: AutoPrunedRetriever-REBEL, which uses REBEL as a triplet parser, and AutoPrunedRetriever-llm, which swaps in an LLM extractor. On GraphRAG-Benchmark (Medical and Novel), both variants achieve state-of-the-art complex reasoning accuracy, improving over HippoRAG2 by roughly 9--11 points, and remain competitive on contextual summarize and generation. On our harder STEM and TV benchmarks, AutoPrunedRetriever again ranks first, while using up to two orders of magnitude fewer tokens than graph-heavy baselines, making it a practical substrate for long-running sessions, evolving corpora, and multi-agent pipelines.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04926v1)
