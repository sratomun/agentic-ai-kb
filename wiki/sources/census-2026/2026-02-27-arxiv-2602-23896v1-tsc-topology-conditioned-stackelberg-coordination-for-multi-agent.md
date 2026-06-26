---
type: source
source_type: arxiv
title: "TSC: Topology-Conditioned Stackelberg Coordination for Multi-Agent Reinforcement Learning in Interactive Driving"
authors: Xiaotong Zhang, Gang Xiong, Yuanjing Wang, Siyu Teng et al.
url: https://arxiv.org/abs/2602.23896v1
date: 2026-02-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.RO
tags: [autonomous-driving-agents, agent-reliability, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# TSC: Topology-Conditioned Stackelberg Coordination for Multi-Agent Reinforcement Learning in Interactive Driving

**arXiv:** [2602.23896v1](https://arxiv.org/abs/2602.23896v1) · 2026-02-27 · cs.RO
**Authors:** Xiaotong Zhang, Gang Xiong, Yuanjing Wang, Siyu Teng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Safe and efficient autonomous driving in dense traffic is fundamentally a decentralized multi-agent coordination problem, where interactions at conflict points such as merging and weaving must be resolved reliably under partial observability. With only local and incomplete cues, interaction patterns can change rapidly, often causing unstable behaviors such as oscillatory yielding or unsafe commitments. Existing multi-agent reinforcement learning (MARL) approaches either adopt synchronous decision-making, which exacerbate non-stationarity, or depend on centralized sequencing mechanisms that scale poorly as traffic density increases. To address these limitations, we propose Topology-conditioned Stackelberg Coordination (TSC), a learning framework for decentralized interactive driving under communication-free execution, which extracts a time-varying directed priority graph from braid-inspired weaving relations between trajectories, thereby defining local leader-follower dependencies without constructing a global order of play. Conditioned on this graph, TSC endogenously factorizes dense interactions into graph-local Stackelberg subgames and, under centralized training and decentralized execution (CTDE), learns a sequential coordination policy that anticipates leaders via action prediction and trains followers through action-conditioned value learning to approximate local best responses, improving training stability and safety in dense traffic. Experiments across four dense traffic scenarios show that TSC achieves superior performance over representative MARL baselines across key metrics, most notably reducing collisions while maintaining competitive traffic efficiency and control smoothness.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.23896v1)
