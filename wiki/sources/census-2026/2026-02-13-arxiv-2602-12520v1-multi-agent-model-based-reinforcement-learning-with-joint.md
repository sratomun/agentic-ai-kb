---
type: source
source_type: arxiv
title: "Multi-Agent Model-Based Reinforcement Learning with Joint State-Action Learned Embeddings"
authors: Zhizun Wang, David Meger
url: https://arxiv.org/abs/2602.12520v1
date: 2026-02-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.LG
tags: [agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Multi-Agent Model-Based Reinforcement Learning with Joint State-Action Learned Embeddings

**arXiv:** [2602.12520v1](https://arxiv.org/abs/2602.12520v1) · 2026-02-13 · cs.LG
**Authors:** Zhizun Wang, David Meger

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Learning to coordinate many agents in partially observable and highly dynamic environments requires both informative representations and data-efficient training. To address this challenge, we present a novel model-based multi-agent reinforcement learning framework that unifies joint state-action representation learning with imaginative roll-outs. We design a world model trained with variational auto-encoders and augment the model using the state-action learned embedding (SALE). SALE is injected into both the imagination module that forecasts plausible future roll-outs and the joint agent network whose individual action values are combined through a mixing network to estimate the joint action-value function. By coupling imagined trajectories with SALE-based action values, the agents acquire a richer understanding of how their choices influence collective outcomes, leading to improved long-term planning and optimization under limited real-environment interactions. Empirical studies on well-established multi-agent benchmarks, including StarCraft II Micro-Management, Multi-Agent MuJoCo, and Level-Based Foraging challenges, demonstrate consistent gains of our method over baseline algorithms and highlight the effectiveness of joint state-action learned embeddings within a multi-agent model-based paradigm.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.12520v1)
