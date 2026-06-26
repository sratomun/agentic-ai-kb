---
type: source
source_type: arxiv
title: "KGLAMP: Knowledge Graph-guided Language model for Adaptive Multi-robot Planning and Replanning"
authors: Chak Lam Shek, Faizan M. Tariq, Sangjae Bae, David Isele et al.
url: https://arxiv.org/abs/2602.04129v2
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# KGLAMP: Knowledge Graph-guided Language model for Adaptive Multi-robot Planning and Replanning

**arXiv:** [2602.04129v2](https://arxiv.org/abs/2602.04129v2) · 2026-02-04 · cs.RO
**Authors:** Chak Lam Shek, Faizan M. Tariq, Sangjae Bae, David Isele et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Heterogeneous multi-robot systems are increasingly used in long-horizon missions requiring coordinated planning across diverse capabilities. However, existing planning approaches struggle to construct accurate symbolic representations and maintain plan consistency in dynamic environments. Classical PDDL planners require manually crafted symbolic models, while LLM-based planners often ignore agent heterogeneity and environmental uncertainty. We introduce KGLAMP, a knowledge-graph-guided LLM planning framework for heterogeneous multi-robot teams. The framework maintains a structured knowledge graph encoding object relations, spatial reachability, and robot capabilities, which guides the LLM in generating accurate PDDL problem specifications. The knowledge graph serves as a persistent, dynamically updated memory that incorporates new observations and triggers replanning upon detecting inconsistencies, enabling symbolic plans to adapt to evolving world states. Experiments on the MAT-THOR benchmark show that KGLAMP improves performance by at least 25.3% over both LLM-only and PDDL-based variants.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04129v2)
