---
type: source
source_type: arxiv
title: "Scaling up Energy-Aware Multi-Agent Reinforcement Learning for Mission-Oriented Drone Networks with Individual Reward"
authors: Changling Li, Ying Li
url: https://arxiv.org/abs/2605.24992v1
date: 2026-05-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 15
primary: cs.NI
tags: [autonomous-driving-agents, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Scaling up Energy-Aware Multi-Agent Reinforcement Learning for Mission-Oriented Drone Networks with Individual Reward

**arXiv:** [2605.24992v1](https://arxiv.org/abs/2605.24992v1) · 2026-05-24 · cs.NI
**Authors:** Changling Li, Ying Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent reinforcement learning (MARL) has shown wide applicability in collaborative systems such as autonomous driving and smart cities for its ability of learning through interaction. With the recent development of drone networks, researchers have also applied MARL to address the trajectory planning problems. However, the dynamic environment and the limited battery capacity are still challenging for using MARL to achieve efficient collaborative task execution. In this paper, we propose an energy-aware MARL model as an attempt to tackle these challenges, leveraging Deep Q-Networks (DQN) with \emph{individual reward functions} driven by the task execution progress and the remaining battery of drones. We conduct a set of simulation studies for the proposed mode and compare it with the shared reward MARL~\cite{Li2022MARL} to explore the impact of credit assignment in MARL. The results indicate that our proposed model can achieve at least 80\% success rate regardless of the task locations and lengths. Similar to the shared reward mode, the individual reward mode can achieve a better success rate when the task density is high, and it can hit nearly a 100\% success rate when task density gets close to 40\%. The true advantage of our proposed model with individual reward is revealed when scaling up the environment. The comparison to the shared reward MARL shows that the our proposed model is more robust towards the change of the environment size and agent numbers. It can achieve higher success rate with fewer steps due to the clarity of the goal which improves energy efficiency even better.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.24992v1)
