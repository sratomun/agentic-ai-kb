---
type: source
source_type: arxiv
title: "Autonomous Knowledge Graph Exploration with Adaptive Breadth-Depth Retrieval"
authors: Joaquín Polonuer, Lucas Vittor, Iñaki Arango, Ayush Noori et al.
url: https://arxiv.org/abs/2601.13969v2
date: 2026-01-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, tool-use, arxiv, auto-ingested]
---

# Autonomous Knowledge Graph Exploration with Adaptive Breadth-Depth Retrieval

**arXiv:** [2601.13969v2](https://arxiv.org/abs/2601.13969v2) · 2026-01-20 · cs.AI
**Authors:** Joaquín Polonuer, Lucas Vittor, Iñaki Arango, Ayush Noori et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieving evidence for language model queries from knowledge graphs requires balancing broad search across the graph with multi-hop traversal to follow relational links. Similarity-based retrievers provide coverage but remain shallow, whereas traversal-based methods rely on selecting seed nodes to start exploration, which can fail when queries span multiple entities and relations. We introduce ARK: Adaptive Retriever of Knowledge, a tool-using KG retriever that gives a language model control over this breadth-depth tradeoff using a two-operation toolset: global lexical search over node descriptors and one-hop neighborhood exploration that composes into multi-hop traversal. ARK alternates between breadth-oriented discovery and depth-oriented expansion without depending on a fragile seed selection, a pre-set hop depth, or requiring retrieval training. ARK adapts tool use to queries, using global search for language-heavy queries and neighborhood exploration for relation-heavy queries. On STaRK, ARK reaches 59.1% average Hit@1 and 67.4 average MRR, improving average Hit@1 by up to 31.4% and average MRR by up to 28.0% over retrieval-based and agent-based training-free methods. Finally, we distill ARK's tool-use trajectories from a large teacher into an 8B model via label-free imitation, improving Hit@1 by +7.0, +26.6, and +13.5 absolute points over the base 8B model on AMAZON, MAG, and PRIME datasets, respectively, while retaining up to 98.5% of the teacher's Hit@1 rate.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.13969v2)
