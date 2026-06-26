---
type: source
source_type: arxiv
title: "CorrectionPlanner: Self-Correction Planner with Reinforcement Learning in Autonomous Driving"
authors: Yihong Guo, Dongqiangzi Ye, Sijia Chen, Anqi Liu et al.
url: https://arxiv.org/abs/2603.15771v1
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.RO
tags: [autonomous-driving-agents, agentic-rl, agent-security, arxiv, auto-ingested]
---

# CorrectionPlanner: Self-Correction Planner with Reinforcement Learning in Autonomous Driving

**arXiv:** [2603.15771v1](https://arxiv.org/abs/2603.15771v1) · 2026-03-16 · cs.RO
**Authors:** Yihong Guo, Dongqiangzi Ye, Sijia Chen, Anqi Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous driving requires safe planning, but most learning-based planners lack explicit self-correction ability: once an unsafe action is proposed, there is no mechanism to correct it. Thus, we propose CorrectionPlanner, an autoregressive planner with self-correction that models planning as motion-token generation within a propose, evaluate, and correct loop. At each planning step, the policy proposes an action, namely a motion token, and a learned collision critic predicts whether it will induce a collision within a short horizon. If the critic predicts a collision, we retain the sequence of historical unsafe motion tokens as a self-correction trace, generate the next motion token conditioned on it, and repeat this process until a safe motion token is proposed or the safety criterion is met. This self-correction trace, consisting of all unsafe motion tokens, represents the planner's correction process in motion-token space, analogous to a reasoning trace in language models. We train the planner with imitation learning followed by model-based reinforcement learning using rollouts from a pretrained world model that realistically models agents' reactive behaviors. Closed-loop evaluations show that CorrectionPlanner reduces collision rate by over 20% on Waymax and achieves state-of-the-art planning scores on nuPlan.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.15771v1)
