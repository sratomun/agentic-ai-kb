---
type: source
source_type: arxiv
title: "SeedER: Seed-and-Expand Retrieval from Knowledge Graphs"
authors: Hamed Shirzad, Frederik Wenkel, Dominique Beaini, Danica J. Sutherland et al.
url: https://arxiv.org/abs/2605.23753v1
date: 2026-05-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.LG
tags: [knowledge-graph, agentic-rl, arxiv, auto-ingested]
---

# SeedER: Seed-and-Expand Retrieval from Knowledge Graphs

**arXiv:** [2605.23753v1](https://arxiv.org/abs/2605.23753v1) · 2026-05-22 · cs.LG
**Authors:** Hamed Shirzad, Frederik Wenkel, Dominique Beaini, Danica J. Sutherland et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Knowledge graphs (KGs) offer a rich representation for relational knowledge, but their irregular structure makes retrieval challenging: ego-graph expansion grows rapidly, and dense embedding methods struggle with multi-hop compositional queries. Existing agent-based graph exploration approaches, while expressive, are often too expensive for large-scale retrieval. We introduce SeedER (Seed-and-Expand Retrieval), a retrieval framework that explicitly leverages KG structure through iterative, low-cost expansion. SeedER first seeds a compact set of core nodes using lightweight dense and entity-based retrieval, then selectively expands this set via a learned graph-aware policy trained with reinforcement learning. This design decomposes global reasoning into reusable local decisions, enabling efficient discovery of query-relevant nodes while tightly controlling expansion cost. We show theoretical limitations of dense retrieval on compositional graph queries, and establish advantages of SeedER from both compositional generalization and graph-constrained submodular optimization perspectives. Empirically, SeedER substantially improves recall with compact candidate sets over strong dense and graph-augmented baselines, making it an effective first-stage retriever for knowledge-intensive reasoning systems.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23753v1)
