---
type: source
source_type: arxiv
title: "OptimusKG: Unifying biomedical knowledge in a modern multimodal graph"
authors: Lucas Vittor, Ayush Noori, Iñaki Arango, Joaquín Polonuer et al.
url: https://arxiv.org/abs/2604.27269v1
date: 2026-04-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 0
primary: cs.AI
tags: [clinical-agents, science-agents, knowledge-graph, arxiv, auto-ingested]
---

# OptimusKG: Unifying biomedical knowledge in a modern multimodal graph

**arXiv:** [2604.27269v1](https://arxiv.org/abs/2604.27269v1) · 2026-04-29 · cs.AI
**Authors:** Lucas Vittor, Ayush Noori, Iñaki Arango, Joaquín Polonuer et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Biomedical knowledge graphs (KGs) are widely used in the life sciences, yet many are derived from unstructured documents and therefore lack schema-level constrains, whereas graphs assembled from structured resources are difficult to harmonize into a unified representation. We present OptimusKG, a multimodal biomedical labeled property graph (LPG) built from structured and semi-structured resources to preserve factual, type-specific metadata across molecular, anatomical, clinical, and environmental domains. OptimusKG contains 190,531 nodes across 10 entity types, 21,813,816 edges across 26 relation types, and 67,249,863 property instances encoding 110,276,843 values across 150 distinct property keys, derived from 18 ontologies and controlled vocabularies. The graph enforces a top-level schema for nodes and edges and retains granular, type-specific properties, cross-references, and provenance across molecular, anatomical, clinical, and environmental domains. We assessed the validity of OptimusKG by evaluating whether graph relationships are supported by evidence from the scientific literature using a multimodal agent, PaperQA3. PaperQA3 identified supporting evidence for 70.0% of sampled edges, whereas 83.4% of sampled false edges received no supporting evidence. Edges without literature support were concentrated in associations derived from experimental and functional genomics resources, suggesting that OptimusKG captures biomedical knowledge that may precede synthesis in the scientific literature. OptimusKG is distributed as Apache Parquet files, providing a standardized resource for graph-based machine learning, knowledge-grounded retrieval with large language models, and biomedical discovery use cases such as hypothesis generation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.27269v1)
