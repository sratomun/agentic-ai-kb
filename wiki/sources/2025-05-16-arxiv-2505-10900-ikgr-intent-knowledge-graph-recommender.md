---
type: source
source_type: arxiv
depth: abstract
title: "Tuning-Free LLM Can Build A Strong Recommender Under Sparse Connectivity And Knowledge Gap Via Extracting Intent"
authors: Wenqing Zheng et al. (Capital One)
url: https://arxiv.org/abs/2505.10900
date: 2025-05-16
venue: Learning on Graphs (LoG) 2025
tags: [intent-grounding, recommendation-agents, knowledge-graph, arxiv, semantic-layer-corpus]
---

# Tuning-Free LLM Can Build A Strong Recommender Under Sparse Connectivity And Knowledge Gap Via Extracting Intent

**arXiv:** [2505.10900](https://arxiv.org/abs/2505.10900) · 2025-05-16 · Learning on Graphs (LoG) 2025
**Authors:** Wenqing Zheng et al. (Capital One)

> Abstract-tier note (extended-search corpus, not in the local agents-centric census). Part of the intent-grounding / semantic-layer thread (2026-06-23).

## Abstract
Recent advances in recommendation with large language models (LLMs) often rely on either commonsense augmentation at the item-category level or implicit intent modeling on existing knowledge graphs. However, such approaches struggle to capture grounded user intents and to handle sparsity and cold-start scenarios. In this work, we present LLM-based Intent Knowledge Graph Recommender (IKGR), a novel framework that constructs an intent-centric knowledge graph where both users and items are explicitly linked to intent nodes extracted by a tuning-free, RAG-guided LLM pipeline. By grounding intents in external knowledge sources and user profiles, IKGR canonically represents what a user seeks and what an item satisfies as first-class entities. To alleviate sparsity, we further introduce a mutual-intent connectivity densification strategy, which shortens semantic paths between users and long-tail items without requiring cross-graph fusion. Finally, a lightweight GNN layer is employed on top of the intent-enhanced graph to produce recommendation signals with low latency. Extensive experiments on public and enterprise datasets demonstrate that IKGR consistently outperforms strong baselines, particularly on cold-start and long-tail slices, while remaining efficient through a fully offline LLM pipeline.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[recommendation-agents|Recommendation agents]] · [[knowledge-graph|Knowledge graph]]
