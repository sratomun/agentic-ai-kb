---
type: source
source_type: arxiv
title: "A Scene Graph Backed Approach to Open Set Semantic Mapping"
authors: Martin Günther, Felix Igelbrink, Oscar Lima, Lennart Niecksch et al.
url: https://arxiv.org/abs/2602.03781v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.RO
tags: [embodied-agents, knowledge-graph, arxiv, auto-ingested]
---

# A Scene Graph Backed Approach to Open Set Semantic Mapping

**arXiv:** [2602.03781v1](https://arxiv.org/abs/2602.03781v1) · 2026-02-03 · cs.RO
**Authors:** Martin Günther, Felix Igelbrink, Oscar Lima, Lennart Niecksch et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Open Set Semantic Mapping and 3D Semantic Scene Graphs (3DSSGs) are established paradigms in robotic perception, deploying them effectively to support high-level reasoning in large-scale, real-world environments remains a significant challenge. Most existing approaches decouple perception from representation, treating the scene graph as a derivative layer generated post hoc. This limits both consistency and scalability. In contrast, we propose a mapping architecture where the 3DSSG serves as the foundational backend, acting as the primary knowledge representation for the entire mapping process. Our approach leverages prior work on incremental scene graph prediction to infer and update the graph structure in real-time as the environment is explored. This ensures that the map remains topologically consistent and computationally efficient, even during extended operations in large-scale settings. By maintaining an explicit, spatially grounded representation that supports both flat and hierarchical topologies, we bridge the gap between sub-symbolic raw sensor data and high-level symbolic reasoning. Consequently, this provides a stable, verifiable structure that knowledge-driven frameworks, ranging from knowledge graphs and ontologies to Large Language Models (LLMs), can directly exploit, enabling agents to operate with enhanced interpretability, trustworthiness, and alignment to human concepts.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03781v1)
