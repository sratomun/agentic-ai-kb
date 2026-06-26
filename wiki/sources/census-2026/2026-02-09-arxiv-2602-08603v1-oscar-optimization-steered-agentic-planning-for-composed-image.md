---
type: source
source_type: arxiv
title: "OSCAR: Optimization-Steered Agentic Planning for Composed Image Retrieval"
authors: Teng Wang, Rong Shan, Jianghao Lin, Junjie Wu et al.
url: https://arxiv.org/abs/2602.08603v1
date: 2026-02-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# OSCAR: Optimization-Steered Agentic Planning for Composed Image Retrieval

**arXiv:** [2602.08603v1](https://arxiv.org/abs/2602.08603v1) · 2026-02-09 · cs.AI
**Authors:** Teng Wang, Rong Shan, Jianghao Lin, Junjie Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Composed image retrieval (CIR) requires complex reasoning over heterogeneous visual and textual constraints. Existing approaches largely fall into two paradigms: unified embedding retrieval, which suffers from single-model myopia, and heuristic agentic retrieval, which is limited by suboptimal, trial-and-error orchestration. To this end, we propose OSCAR, an optimization-steered agentic planning framework for composed image retrieval. We are the first to reformulate agentic CIR from a heuristic search process into a principled trajectory optimization problem. Instead of relying on heuristic trial-and-error exploration, OSCAR employs a novel offline-online paradigm. In the offline phase, we model CIR via atomic retrieval selection and composition as a two-stage mixed-integer programming problem, mathematically deriving optimal trajectories that maximize ground-truth coverage for training samples via rigorous boolean set operations. These trajectories are then stored in a golden library to serve as in-context demonstrations for online steering of VLM planner at online inference time. Extensive experiments on three public benchmarks and a private industrial benchmark show that OSCAR consistently outperforms SOTA baselines. Notably, it achieves superior performance using only 10% of training data, demonstrating strong generalization of planning logic rather than dataset-specific memorization.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.08603v1)
