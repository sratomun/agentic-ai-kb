---
type: source
source_type: arxiv
title: "MemReread: Enhancing Agentic Long-Context Reasoning via Memory-Guided Rereading"
authors: Baibei Ji, Xiaoyang Weng, Juntao Li, Zecheng Tang et al.
url: https://arxiv.org/abs/2605.10268v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# MemReread: Enhancing Agentic Long-Context Reasoning via Memory-Guided Rereading

**arXiv:** [2605.10268v1](https://arxiv.org/abs/2605.10268v1) · 2026-05-11 · cs.CL
**Authors:** Baibei Ji, Xiaoyang Weng, Juntao Li, Zecheng Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
To tackle long-context reasoning tasks without the quadratic complexity of standard attention mechanisms, approaches based on agent memory have emerged, which typically maintain a dynamically updated memory when linearly processing document chunks. To mitigate the potential loss of latent evidence in this memorize-while-reading paradigm, recent works have integrated retrieval modules that allow agents to recall information previously discarded during memory overwriting. However, retrieval-based recall suffers from both evidence loss during memory formation and interference induced by invalid queries. To overcome these limitations, we propose MemReread. Built upon streaming reading, MemReread circumvents intermediate retrieval. It triggers question decomposition and rereading when the final memory is insufficient, enabling the recovery of indirect facts that were prematurely discarded. This design supports non-linear reasoning while preserving the inherent logical flow of document comprehension. To further enhance practicality, we introduce a reinforcement learning framework that enhances length extrapolation capability while dynamically determining the number of rereading passes based on task complexity, thereby flexibly controlling computational overhead. Extensive experiments demonstrate that MemReread consistently outperforms baseline frameworks on long-context reasoning tasks, while maintaining linear time complexity with respect to context length.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10268v1)
