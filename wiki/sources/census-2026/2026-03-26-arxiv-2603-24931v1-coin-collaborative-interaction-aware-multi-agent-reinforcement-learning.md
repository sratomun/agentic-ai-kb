---
type: source
source_type: arxiv
title: "COIN: Collaborative Interaction-Aware Multi-Agent Reinforcement Learning for Self-Driving Systems"
authors: Yifeng Zhang, Jieming Chen, Tingguang Zhou, Tanishq Duhan et al.
url: https://arxiv.org/abs/2603.24931v1
date: 2026-03-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.RO
tags: [autonomous-driving-agents, embodied-agents, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# COIN: Collaborative Interaction-Aware Multi-Agent Reinforcement Learning for Self-Driving Systems

**arXiv:** [2603.24931v1](https://arxiv.org/abs/2603.24931v1) · 2026-03-26 · cs.RO
**Authors:** Yifeng Zhang, Jieming Chen, Tingguang Zhou, Tanishq Duhan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-Agent Self-Driving (MASD) systems provide an effective solution for coordinating autonomous vehicles to reduce congestion and enhance both safety and operational efficiency in future intelligent transportation systems. Multi-Agent Reinforcement Learning (MARL) has emerged as a promising approach for developing advanced end-to-end MASD systems. However, achieving efficient and safe collaboration in dynamic MASD systems remains a significant challenge in dense scenarios with complex agent interactions. To address this challenge, we propose a novel collaborative(CO-) interaction-aware(-IN) MARL framework, named COIN. Specifically, we develop a new counterfactual individual-global twin delayed deep deterministic policy gradient (CIG-TD3) algorithm, crafted in a "centralized training, decentralized execution" (CTDE) manner, which aims to jointly optimize the individual objectives (navigation) and the global objectives (collaboration) of agents. We further introduce a dual-level interaction-aware centralized critic architecture that captures both local pairwise interactions and global system-level dependencies, enabling more accurate global value estimation and improved credit assignment for collaborative policy learning. We conduct extensive simulation experiments in dense urban traffic environments, which demonstrate that COIN consistently outperforms other advanced baseline methods in both safety and efficiency across various system sizes. These results highlight its superiority in complex and dynamic MASD scenarios, as further validated through real-world robot demonstrations. Supplementary videos are available at https://marmotlab.github.io/COIN/

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.24931v1)
