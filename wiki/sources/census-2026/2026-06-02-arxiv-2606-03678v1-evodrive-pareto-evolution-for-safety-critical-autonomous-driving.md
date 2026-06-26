---
type: source
source_type: arxiv
title: "EvoDrive: Pareto Evolution for Safety-Critical Autonomous Driving via Self-Improving LLM Agents"
authors: Tong Nie, Yuewen Mei, Yihong Tang, Junlin He et al.
url: https://arxiv.org/abs/2606.03678v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [autonomous-driving-agents, self-evolving-agents, agent-security, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# EvoDrive: Pareto Evolution for Safety-Critical Autonomous Driving via Self-Improving LLM Agents

**arXiv:** [2606.03678v1](https://arxiv.org/abs/2606.03678v1) · 2026-06-02 · cs.AI
**Authors:** Tong Nie, Yuewen Mei, Yihong Tang, Junlin He et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generating safety-critical scenarios is essential for validating and improving autonomous driving systems, yet it inherently requires maximizing adversariality to expose failures while preserving realism. Existing methods usually manage this trade-off with handcrafted heuristics, confining generation to known priors and overlooking underexplored patterns. While recent open-ended agentic evolution can push this limit, unconstrained general agents lack strict simulator grounding and tend to collapse the multi-objective tension into single-scalar maximization. Here we present EvoDrive, the first automated, LLM-based agentic evolution framework for multi-objective scenario generation. EvoDrive employs a simulator-grounded actor-critic architecture where a memory-driven actor iteratively proposes improvements to the generators and critics filter out implausible candidates, and a self-evolving world evaluator routes promising proposals to optimize simulation budgets. EvoDrive further maintains a Pareto archive of evaluated candidates to preserve diverse attack-realism trade-offs and guide future evolution via simulation feedback. Benchmark results on MetaDrive and CARLA show that EvoDrive not only significantly expands the Pareto frontier across various generators, but also produces valuable scenarios for policy training.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03678v1)
