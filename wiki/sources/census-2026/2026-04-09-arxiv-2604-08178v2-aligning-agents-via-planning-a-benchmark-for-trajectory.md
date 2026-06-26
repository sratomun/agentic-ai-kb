---
type: source
source_type: arxiv
title: "Aligning Agents via Planning: A Benchmark for Trajectory-Level Reward Modeling"
authors: Jiaxuan Wang, Yulan Hu, Wenjin Yang, Zheng Pan et al.
url: https://arxiv.org/abs/2604.08178v2
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, agent-reliability, agentic-rl, agent-security, agent-protocols, arxiv, auto-ingested]
---

# Aligning Agents via Planning: A Benchmark for Trajectory-Level Reward Modeling

**arXiv:** [2604.08178v2](https://arxiv.org/abs/2604.08178v2) · 2026-04-09 · cs.AI
**Authors:** Jiaxuan Wang, Yulan Hu, Wenjin Yang, Zheng Pan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
In classical Reinforcement Learning from Human Feedback (RLHF), Reward Models (RMs) serve as the fundamental signal provider for model alignment. As Large Language Models evolve into agentic systems capable of autonomous tool invocation and complex reasoning, the paradigm of reward modeling faces unprecedented challenges -- most notably, the lack of benchmarks specifically designed to assess RM capabilities within tool-integrated environments. To address this gap, we present Plan-RewardBench, a trajectory-level preference benchmark designed to evaluate how well judges distinguish preferred versus distractor agent trajectories in complex tool-using scenarios. Plan-RewardBench covers four representative task families -- (i) Safety Refusal, (ii) Tool-Irrelevance / Unavailability, (iii) Complex Planning, and (iv) Robust Error Recovery -- comprising validated positive trajectories and confusable hard negatives constructed via multi-model natural rollouts, rule-based perturbations, and minimal-edit LLM perturbations. We benchmark representative RMs (generative, discriminative, and LLM-as-Judge) under a unified pairwise protocol, reporting accuracy trends across varying trajectory lengths and task categories. Furthermore, we provide diagnostic analyses of prevalent failure modes. Our results reveal that all three evaluator families face substantial challenges, with performance degrading sharply on long-horizon trajectories, underscoring the necessity for specialized training in agentic, trajectory-level reward modeling. Ultimately, Plan-RewardBench aims to serve as both a practical evaluation suite and a reusable blueprint for constructing agentic planning preference data.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.08178v2)
