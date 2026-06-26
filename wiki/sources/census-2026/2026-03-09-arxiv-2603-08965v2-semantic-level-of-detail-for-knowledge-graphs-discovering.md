---
type: source
source_type: arxiv
title: "Semantic Level of Detail for Knowledge Graphs: Discovering Abstraction Boundaries via Spectral Heat Diffusion"
authors: Edward Izgorodin
url: https://arxiv.org/abs/2603.08965v2
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 1
primary: cs.LG
tags: [knowledge-graph, arxiv, auto-ingested]
---

# Semantic Level of Detail for Knowledge Graphs: Discovering Abstraction Boundaries via Spectral Heat Diffusion

**arXiv:** [2603.08965v2](https://arxiv.org/abs/2603.08965v2) · 2026-03-09 · cs.LG
**Authors:** Edward Izgorodin

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Graph-structured knowledge systems -- from knowledge graphs to GraphRAG pipelines -- organize information into hierarchical communities, yet lack a principled mechanism for continuous resolution control: where do the qualitative boundaries between abstraction levels lie, and how should an agent navigate them? Current approaches rely on discrete community detection with manually tuned resolution parameters (e.g., Leiden $γ$), offering no continuous zoom and no formal guarantees. We introduce Semantic Level of Detail (SLoD), a framework that addresses both problems by defining a continuous zoom operator via heat kernel diffusion on a graph Laplacian whose kNN structure is induced by a Poincare-ball embedding. We prove hierarchical coherence in the tree limit (exact tree with Sarkar embedding), with bounded approximation error, and demonstrate consistent boundary-detection behaviour on noisy hierarchies; spectral gaps in the graph Laplacian then induce emergent scale boundaries -- scales where the representation undergoes qualitative transitions -- detectable without manual resolution tuning. On synthetic hierarchies (HSBM, 1024 nodes), spectral clustering at the BoundaryScan-detected scale recovers planted levels, with macro ARI saturating at 1.00 in the high-SNR regime (50-seed median) and meso ARI reaching 0.89 [0.86, 0.92] at r=200. On the full WordNet noun hierarchy (82K synsets), using 100 stratified leaf queries, detected boundaries align with true taxonomic depth ($τ= 0.79$), demonstrating meaningful abstraction-level discovery in real-world knowledge graphs without resolution-parameter tuning. The composite weights, MAD threshold, and kNN-parameter rule ($k = \max(10, \min(\lfloor\sqrt{N}\rfloor, 50))$) use defaults that transferred unchanged between HSBM and WordNet; their behaviour on graphs with implicit or qualitatively different hierarchical structure is open.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08965v2)
