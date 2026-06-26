---
type: source
source_type: arxiv
title: "IdeaForge: A Knowledge Graph-Grounded Multi-Agent Framework for Cross-Methodology Innovation Analysis and Patent Claim Generation"
authors: Joy Bose
url: https://arxiv.org/abs/2605.13311v1
date: 2026-05-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.AI
tags: [knowledge-graph, multi-agent-systems, arxiv, auto-ingested]
---

# IdeaForge: A Knowledge Graph-Grounded Multi-Agent Framework for Cross-Methodology Innovation Analysis and Patent Claim Generation

**arXiv:** [2605.13311v1](https://arxiv.org/abs/2605.13311v1) · 2026-05-13 · cs.AI
**Authors:** Joy Bose

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current AI-assisted innovation systems typically apply a single ideation methodology (such as TRIZ or Design Thinking) using sequential prompt-based workflows that do not preserve intermediate reasoning structure. As a result, insights generated across methodologies remain fragmented, limiting traceability, synthesis, and systematic evaluation of novelty. We present IdeaForge, a knowledge graph-grounded multi-agent framework for innovation analysis and patent claim generation. IdeaForge integrates multiple innovation methodologies (TRIZ, Design Thinking, and SCAMPER) through specialist agents operating over a persistent FalkorDB knowledge graph. Each agent contributes structured entities and relationships representing contradictions, inventive principles, user needs, transformations, analogies, and candidate claims. The central contribution of IdeaForge is a cross-methodology convergence mechanism implemented through graph-based claim linkage. Claims independently supported by multiple methodologies are connected using CONVERGENT relationships, enabling identification of high-confidence innovation candidates through graph traversal. A downstream patent drafting agent generates structured patent drafts grounded in convergent claim subgraphs, reducing reliance on unconstrained language model generation. An InnovationScore formula ranks claims by convergent support, methodology diversity, claim strength, and prior art challenge count. We describe the graph schema, agent architecture, convergence detection pipeline, and patent synthesis workflow. Experiments on a legal technology use case demonstrate that graph-grounded multi-methodology synthesis produces more diverse and traceable innovation candidates compared to single-methodology baselines. We discuss implications for computational creativity, explainable AI-assisted invention, and graph-native innovation systems.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.13311v1)
