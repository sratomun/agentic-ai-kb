---
type: source
source_type: arxiv
title: "MAVEN-T: Reinforced Heterogeneous Distillation for Real-Time Multi-Agent Trajectory Prediction"
authors: Wenchang Duan, Zhenguo Gao, Jinguo Xian, Yi Shi
url: https://arxiv.org/abs/2604.10169v3
date: 2026-04-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [autonomous-driving-agents, agent-reliability, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# MAVEN-T: Reinforced Heterogeneous Distillation for Real-Time Multi-Agent Trajectory Prediction

**arXiv:** [2604.10169v3](https://arxiv.org/abs/2604.10169v3) · 2026-04-11 · cs.AI
**Authors:** Wenchang Duan, Zhenguo Gao, Jinguo Xian, Yi Shi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Trajectory prediction is a key component of autonomous driving systems because future motions directly affect collision checking, behavior planning, and control. The task remains challenging under dense interactions, heterogeneous behaviors, multimodal futures, and limited on-board computation. Existing graph, attention, and generative predictors improve interaction reasoning or uncertainty modeling, but their high-capacity designs are often costly for real-time deployment. Lightweight predictors and conventional distillation reduce inference cost, yet usually rely on static imitation and do not explicitly correct safety-relevant teacher bias. This paper proposes \textbf{MAVEN-T}, a reinforced heterogeneous distillation framework for real-time multi-agent trajectory prediction. A high-capacity teacher models directed local interactions with a surround-aware graph encoder, combines efficient temporal filtering with shifted-window spatial attention, and decodes maneuver-specific futures through a sparse Mixture-of-Experts head. A compact GRU--Squeeze-and-Excitation student with a Low-Rank Adapted policy head is trained by feature-, attention-, and semantic-level distillation. To align prediction with downstream behavior, the student is further refined by Proximal Policy Optimization rewards for collision avoidance, comfort, and progress, while a complexity-aware curriculum and Elastic Weight Consolidation stabilize stage-wise training. Experiments on NGSIM, HighD, MoCAD, Argoverse~2, and the Waymo Open Motion Dataset evaluate accuracy, efficiency, generalization, robustness, and closed-loop safety. The student achieves 6.2$\times$ parameter compression, 3.7$\times$ inference acceleration, and 14.6,ms latency on an NVIDIA Jetson AGX Orin while maintaining competitive accuracy.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10169v3)
