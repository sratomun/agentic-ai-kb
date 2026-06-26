---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "On-device Semantic Selection Made Low Latency and Memory Efficient with Monolithic Forwarding"
authors: Jiahao Zhou et al.
url: https://arxiv.org/abs/2510.15620v2
date: 2025-10-17
score: 3
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, agent-memory, llm-as-judge, agentic-rag, recommendation-agents]
---

# On-device Semantic Selection Made Low Latency and Memory Efficient with Monolithic Forwarding

**arXiv:** [2510.15620v2](https://arxiv.org/abs/2510.15620v2) · 2025-10-17 · cs.LG
**Authors:** Jiahao Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Semantic top-K selection with cross-encoder rerankers underpins on-device AI services, such as retrieval-augmented generation, agent memory, and personalized recommendation. However, its latency and memory demands dominate end-to-end budgets on edge hardware. Revisiting the objective of top-K selection, we reveal that only relative rankings matter, not exact per-candidate scores. We further observe sequence-level sparsity: relative rankings progressively stabilize in intermediate layers, enabling early pruning prior to completing full inference. Building on this insight, we propose monolithic forwarding and develop a training-free inference system, PRISM. By maintaining a global view of all candidates, it reduces latency through progressive cluster pruning. It also bounds peak memory usage by strategically overlapping I/O with computation via overlapped layer streaming and chunked execution. We evaluate PRISM against state-of-the-art baselines on rerankers from 0.6 B to 8 B parameters across Apple M2 and RTX 5070. PRISM consistently reduces latency by up to 89.2% and peak memory by up to 91.3% in microbenchmarks, without compromising precision. Across three real-world on-device AI applications, PRISM lowers latency by 11.6%-51.0% and peak memory by 18.6%-77.8%, demonstrating substantial improvements in efficiency and deployability.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[llm-as-judge]] · [[agentic-rag]] · [[recommendation-agents]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2510.15620v2)
