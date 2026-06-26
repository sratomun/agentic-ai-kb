---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Compiling Deterministic Structure into SLM Harnesses"
authors: Zan Kai Chong et al.
url: https://arxiv.org/abs/2604.17450v3
date: 2026-04-19
score: 7
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, reasoning-models]
---

# Compiling Deterministic Structure into SLM Harnesses

**arXiv:** [2604.17450v3](https://arxiv.org/abs/2604.17450v3) · 2026-04-19 · cs.AI
**Authors:** Zan Kai Chong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enterprise SLM deployment faces epistemic asymmetry: small models cannot self-correct reasoning errors, while frontier LLMs incur prohibitive costs and data sovereignty risks at scale. We propose Semantic Gradient Descent (SGDe), a teacher-student framework that compiles agentic workflows into discrete execution plans--DAG topologies, system prompts, and deterministic code. The trailing e distinguishes this discrete, compilation-based approach from stochastic gradient descent. Operating in discrete semantic space, a frontier teacher generates natural-language critiques that serve as directional gradients to iteratively refine the SLM's workflow artefacts. We formalise SGDe under PAC learning, establishing sample-complexity bounds that enable convergence with as few as three training examples by leveraging the teacher as a statistical prior. On an adversarially synthesized GSM-Hard test set, compiled workflows achieve 91.3% accuracy at m=5 and 99.3% at m=3--a +26.3% to +34.3% absolute gain over state-of-the-art prompt optimisers. Within harness engineering, SGDe treats deterministic code placement (which subtasks to delegate to Python versus retain as LLM calls) as a trace-driven, per-node optimisation target, generalising static whole-problem offloading in PAL and PoT. The teacher compiles two deterministic structures: capability offloading (delegating subtasks to Python when the SLM is unreliable) and structural consensus (wrapping variance-sensitive steps in fan-out/fan-in subgraphs with deterministic voting).

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17450v3)
