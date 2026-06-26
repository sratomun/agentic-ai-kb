---
type: source
source_type: arxiv
title: "Memora: A Harmonic Memory Representation Balancing Abstraction and Specificity"
authors: Menglin Xia, Xuchao Zhang, Shantanu Dixit, Paramaguru Harimurugan et al.
url: https://arxiv.org/abs/2602.03315v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.AI
tags: [knowledge-graph, agentic-rag, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Memora: A Harmonic Memory Representation Balancing Abstraction and Specificity

**arXiv:** [2602.03315v1](https://arxiv.org/abs/2602.03315v1) · 2026-02-03 · cs.AI
**Authors:** Menglin Xia, Xuchao Zhang, Shantanu Dixit, Paramaguru Harimurugan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agent memory systems must accommodate continuously growing information while supporting efficient, context-aware retrieval for downstream tasks. Abstraction is essential for scaling agent memory, yet it often comes at the cost of specificity, obscuring the fine-grained details required for effective reasoning. We introduce Memora, a harmonic memory representation that structurally balances abstraction and specificity. Memora organizes information via its primary abstractions that index concrete memory values and consolidate related updates into unified memory entries, while cue anchors expand retrieval access across diverse aspects of the memory and connect related memories. Building on this structure, we employ a retrieval policy that actively exploits these memory connections to retrieve relevant information beyond direct semantic similarity. Theoretically, we show that standard Retrieval-Augmented Generation (RAG) and Knowledge Graph (KG)-based memory systems emerge as special cases of our framework. Empirically, Memora establishes a new state-of-the-art on the LoCoMo and LongMemEval benchmarks, demonstrating better retrieval relevance and reasoning effectiveness as memory scales.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03315v1)
