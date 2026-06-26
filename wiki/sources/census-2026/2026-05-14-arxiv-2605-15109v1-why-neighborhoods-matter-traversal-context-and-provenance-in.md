---
type: source
source_type: arxiv
title: "Why Neighborhoods Matter: Traversal Context and Provenance in Agentic GraphRAG"
authors: Riccardo Terrenzi, Maximilian von Zastrow, Serkan Ayvaz
url: https://arxiv.org/abs/2605.15109v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, agentic-rag, arxiv, auto-ingested]
---

# Why Neighborhoods Matter: Traversal Context and Provenance in Agentic GraphRAG

**arXiv:** [2605.15109v1](https://arxiv.org/abs/2605.15109v1) · 2026-05-14 · cs.AI
**Authors:** Riccardo Terrenzi, Maximilian von Zastrow, Serkan Ayvaz

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation can improve factuality by grounding answers in external evidence, but Agentic GraphRAG complicates what it means for citations to be faithful. In these systems, an agent explores a knowledge graph before producing an answer and a small set of citations. We frame citation faithfulness as a trajectory-level problem: final citations should not only support the answer, but also account for the graph traversal, structure, and visited-but-uncited entities that may influence it. Through controlled ablation experiments, we compare the effects of isolating, removing, and masking cited and uncited graph entities. Our results show that cited evidence is often necessary, as removing it substantially changes answers and reduces accuracy. However, citations are not sufficient, because accurate answers can also depend on uncited traversal context and surrounding graph structure. These findings suggest that citation evaluation in Agentic GraphRAG should move beyond source support toward provenance over the broader retrieval trajectory.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15109v1)
