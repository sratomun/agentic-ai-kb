---
type: source
source_type: arxiv
title: "Beyond Self-Play and Scale: A Behavior Benchmark for Generalization in Autonomous Driving"
authors: Aron Distelzweig, Faris Janjoš, Andreas Look, Anna Rothenhäusler et al.
url: https://arxiv.org/abs/2605.10034v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.RO
tags: [autonomous-driving-agents, self-evolving-agents, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Beyond Self-Play and Scale: A Behavior Benchmark for Generalization in Autonomous Driving

**arXiv:** [2605.10034v1](https://arxiv.org/abs/2605.10034v1) · 2026-05-11 · cs.RO
**Authors:** Aron Distelzweig, Faris Janjoš, Andreas Look, Anna Rothenhäusler et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent Autonomous Driving (AD) works such as GigaFlow and PufferDrive have unlocked Reinforcement Learning (RL) at scale as a training strategy for driving policies. Yet such policies remain disconnected from established benchmarks, leaving the performance of large-scale RL for driving on standardized evaluations unknown. We present BehaviorBench -- a comprehensive test suite that closes this gap along three axes: Evaluation, Complexity, and Behavior Diversity. In terms of Evaluation, we provide an interface connecting PufferDrive to nuPlan, which, for the first time, enables policies trained via RL at scale to be evaluated on an established planning benchmark for autonomous driving. Complementarily, we offer an evaluation framework that allows planners to be benchmarked directly inside the PufferDrive simulation, at a fraction of the time. Regarding Complexity, we observe that today's standardized benchmarks are so simple that near-perfect scores are achievable by straight lane following with collision checking. We extract a meaningful, interaction-rich split from the Waymo Open Motion Dataset (WOMD) on which strong performance is impossible without multi-agent reasoning. Lastly, we address Behavior Diversity. Existing benchmarks commonly evaluate planners against a single rule-based traffic model, the Intelligent Driver Model (IDM). We provide a diverse suite of interactive traffic agents to stress-test policies under heterogeneous behaviors, beyond just using IDM. Overall, our benchmarking analysis uncovers the following insight: despite learning interactive behaviors in an emergent manner, policies trained via pure self-play under standard reward functions overfit to their training opponents and fail to generalize to other traffic agent behaviors. Building on this observation, we propose a hybrid planner that combines a PPO policy with a rule-based planner.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[ppo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10034v1)
