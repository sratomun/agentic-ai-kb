---
type: source
source_type: arxiv
title: "PerlAD: Towards Enhanced Closed-loop End-to-end Autonomous Driving with Pseudo-simulation-based Reinforcement Learning"
authors: Yinfeng Gao, Qichao Zhang, Deqing Liu, Zhongpu Xia et al.
url: https://arxiv.org/abs/2603.14908v1
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.RO
tags: [autonomous-driving-agents, agent-reliability, agentic-rl, agent-security, agent-evaluation, arxiv, auto-ingested]
---

# PerlAD: Towards Enhanced Closed-loop End-to-end Autonomous Driving with Pseudo-simulation-based Reinforcement Learning

**arXiv:** [2603.14908v1](https://arxiv.org/abs/2603.14908v1) · 2026-03-16 · cs.RO
**Authors:** Yinfeng Gao, Qichao Zhang, Deqing Liu, Zhongpu Xia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
End-to-end autonomous driving policies based on Imitation Learning (IL) often struggle in closed-loop execution due to the misalignment between inadequate open-loop training objectives and real driving requirements. While Reinforcement Learning (RL) offers a solution by directly optimizing driving goals via reward signals, the rendering-based training environments introduce the rendering gap and are inefficient due to high computational costs. To overcome these challenges, we present a novel Pseudo-simulation-based RL method for closed-loop end-to-end autonomous driving, PerlAD. Based on offline datasets, PerlAD constructs a pseudo-simulation that operates in vector space, enabling efficient, rendering-free trial-and-error training. To bridge the gap between static datasets and dynamic closed-loop environments, PerlAD introduces a prediction world model that generates reactive agent trajectories conditioned on the ego vehicle's plan. Furthermore, to facilitate efficient planning, PerlAD utilizes a hierarchical decoupled planner that combines IL for lateral path generation and RL for longitudinal speed optimization. Comprehensive experimental results demonstrate that PerlAD achieves state-of-the-art performance on the Bench2Drive benchmark, surpassing the previous E2E RL method by 10.29% in Driving Score without requiring expensive online interactions. Additional evaluations on the DOS benchmark further confirm its reliability in handling safety-critical occlusion scenarios.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.14908v1)
