---
type: source
source_type: arxiv
title: "Enhancing Vision-Language Navigation with Multimodal Event Knowledge from Real-World Indoor Tour Videos"
authors: Haoxuan Xu, Tianfu Li, Wenbo Chen, Yi Liu et al.
url: https://arxiv.org/abs/2602.23937v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Enhancing Vision-Language Navigation with Multimodal Event Knowledge from Real-World Indoor Tour Videos

**arXiv:** [2602.23937v1](https://arxiv.org/abs/2602.23937v1) · 2026-02-27 · cs.RO
**Authors:** Haoxuan Xu, Tianfu Li, Wenbo Chen, Yi Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Vision-Language Navigation (VLN) agents often struggle with long-horizon reasoning in unseen environments, particularly when facing ambiguous, coarse-grained instructions. While recent advances use knowledge graph to enhance reasoning, the potential of multimodal event knowledge inspired by human episodic memory remains underexplored. In this work, we propose an event-centric knowledge enhancement strategy for automated process knowledge mining and feature fusion to solve coarse-grained instruction and long-horizon reasoning in VLN task. First, we construct YE-KG, the first large-scale multimodal spatiotemporal knowledge graph, with over 86k nodes and 83k edges, derived from real-world indoor videos. By leveraging multimodal large language models (i.e., LLaVa, GPT4), we extract unstructured video streams into structured semantic-action-effect events to serve as explicit episodic memory. Second, we introduce STE-VLN, which integrates the above graph into VLN models via a Coarse-to-Fine Hierarchical Retrieval mechanism. This allows agents to retrieve causal event sequences and dynamically fuse them with egocentric visual observations. Experiments on REVERIE, R2R, and R2R-CE benchmarks demonstrate the efficiency of our event-centric strategy, outperforming state-of-the-art approaches across diverse action spaces. Our data and code are available on the project website https://sites.google.com/view/y-event-kg/.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23937v1)
