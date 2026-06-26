---
type: source
source_type: arxiv
title: "Hippocampus: An Efficient and Scalable Memory Module for Agentic AI"
authors: Yi Li, Lianjie Cao, Faraz Ahmed, Puneet Sharma et al.
url: https://arxiv.org/abs/2602.13594v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Hippocampus: An Efficient and Scalable Memory Module for Agentic AI

**arXiv:** [2602.13594v1](https://arxiv.org/abs/2602.13594v1) · 2026-02-14 · cs.AI
**Authors:** Yi Li, Lianjie Cao, Faraz Ahmed, Puneet Sharma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic AI require persistent memory to store user-specific histories beyond the limited context window of LLMs. Existing memory systems use dense vector databases or knowledge-graph traversal (or hybrid), incurring high retrieval latency and poor storage scalability. We introduce Hippocampus, an agentic memory management system that uses compact binary signatures for semantic search and lossless token-ID streams for exact content reconstruction. Its core is a Dynamic Wavelet Matrix (DWM) that compresses and co-indexes both streams to support ultra-fast search in the compressed domain, thus avoiding costly dense-vector or graph computations. This design scales linearly with memory size, making it suitable for long-horizon agentic deployments. Empirically, our evaluation shows that Hippocampus reduces end-to-end retrieval latency by up to 31$\times$ and cuts per-query token footprint by up to 14$\times$, while maintaining accuracy on both LoCoMo and LongMemEval benchmarks.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13594v1)
