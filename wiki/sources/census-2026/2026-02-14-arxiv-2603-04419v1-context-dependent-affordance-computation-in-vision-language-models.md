---
type: source
source_type: arxiv
title: "Context-Dependent Affordance Computation in Vision-Language Models"
authors: Murad Farzulla
url: https://arxiv.org/abs/2603.04419v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.CL
tags: [embodied-agents, knowledge-graph, arxiv, auto-ingested]
---

# Context-Dependent Affordance Computation in Vision-Language Models

**arXiv:** [2603.04419v1](https://arxiv.org/abs/2603.04419v1) · 2026-02-14 · cs.CL
**Authors:** Murad Farzulla

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We characterize the phenomenon of context-dependent affordance computation in vision-language models (VLMs). Through a large-scale computational study (n=3,213 scene-context pairs from COCO-2017) using Qwen-VL 30B and LLaVA-1.5-13B subject to systematic context priming across 7 agentic personas, we demonstrate massive affordance drift: mean Jaccard similarity between context conditions is 0.095 (95% CI: [0.093, 0.096], p < 0.0001), indicating that >90% of lexical scene description is context-dependent. Sentence-level cosine similarity confirms substantial drift at the semantic level (mean = 0.415, 58.5% context-dependent). Stochastic baseline experiments (2,384 inference runs across 4 temperatures and 5 seeds) confirm this drift reflects genuine context effects rather than generation noise: within-prime variance is substantially lower than cross-prime variance across all conditions. Tucker decomposition with bootstrap stability analysis (n=1,000 resamples) reveals stable orthogonal latent factors: a "Culinary Manifold" isolated to chef contexts and an "Access Axis" spanning child-mobility contrasts. These findings establish that VLMs compute affordances in a substantially context-dependent manner -- with the difference between lexical (90%) and semantic (58.5%) measures reflecting that surface vocabulary changes more than underlying meaning under context shifts -- and suggest a direction for robotics research: dynamic, query-dependent ontological projection (JIT Ontology) rather than static world modeling. We do not claim to establish processing order or architectural primacy; such claims require internal representational analysis beyond output behavior.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.04419v1)
