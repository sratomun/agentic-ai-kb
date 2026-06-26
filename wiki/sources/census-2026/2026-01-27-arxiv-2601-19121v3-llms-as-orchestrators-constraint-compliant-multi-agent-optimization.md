---
type: source
source_type: arxiv
title: "LLMs as Orchestrators: Constraint-Compliant Multi-Agent Optimization for Recommendation Systems"
authors: Guilin Zhang, Kai Zhao, Jeffrey Friedman, Xu Chu
url: https://arxiv.org/abs/2601.19121v3
date: 2026-01-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.IR
tags: [recommendation-agents, multi-agent-systems, arxiv, auto-ingested]
---

# LLMs as Orchestrators: Constraint-Compliant Multi-Agent Optimization for Recommendation Systems

**arXiv:** [2601.19121v3](https://arxiv.org/abs/2601.19121v3) · 2026-01-27 · cs.IR
**Authors:** Guilin Zhang, Kai Zhao, Jeffrey Friedman, Xu Chu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recommendation systems must optimize multiple objectives while satisfying hard business constraints such as fairness and coverage. For example, an e-commerce platform may require every recommendation list to include items from multiple sellers and at least one newly listed product; violating such constraints--even once--is unacceptable in production. Prior work on multi-objective recommendation and recent LLM-based recommender agents largely treat constraints as soft penalties or focus on item scoring and interaction, leading to frequent violations in real-world deployments. How to leverage LLMs for coordinating constrained optimization in recommendation systems remains underexplored. We propose DualAgent-Rec, an LLM-coordinated dual-agent framework for constrained multi-objective e-commerce recommendation. The framework separates optimization into an Exploitation Agent that prioritizes accuracy under hard constraints and an Exploration Agent that promotes diversity through unconstrained Pareto search. An LLM-based coordinator adaptively allocates resources between agents based on optimization progress and constraint satisfaction, while an adaptive epsilon-relaxation mechanism guarantees feasibility of final solutions. Experiments on the Amazon Reviews 2023 dataset demonstrate that DualAgent-Rec achieves 100% constraint satisfaction and improves Pareto hypervolume by 4-6% over strong baselines, while maintaining competitive accuracy-diversity trade-offs. These results indicate that LLMs can act as effective orchestration agents for deployable and constraint-compliant recommendation systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.19121v3)
