---
type: source
source_type: arxiv
title: "MAPLE: Latent Multi-Agent Play for End-to-End Autonomous Driving"
authors: Rajeev Yasarla, Deepti Hegde, Hsin-Pai Cheng, Shizhong Han et al.
url: https://arxiv.org/abs/2605.14201v2
date: 2026-05-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.RO
tags: [autonomous-driving-agents, embodied-agents, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# MAPLE: Latent Multi-Agent Play for End-to-End Autonomous Driving

**arXiv:** [2605.14201v2](https://arxiv.org/abs/2605.14201v2) · 2026-05-13 · cs.RO
**Authors:** Rajeev Yasarla, Deepti Hegde, Hsin-Pai Cheng, Shizhong Han et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Vision-language-action (VLA) models are effective as end-to-end motion planners, but can be brittle when evaluated in closed-loop settings due to being trained under traditional imitation learning framework. Existing closed-loop supervision approaches lack scalability and fail to completely model a reactive environment. We propose MAPLE, a novel framework for reactive, multi-agent rollout of a dynamic driving scenario in the latent space of the VLA model. The ego vehicle and nearby traffic agents are independently controlled over multi-step horizons, while being reactive to other agents in the scene, enabling closed-loop training. MAPLE consists of two training stages: (1) supervised fine-tuning on the latent rollouts based on ground-truth trajectories, followed by (2) reinforcement learning with global and agent -specific rewards that encourage safety, progress, and interaction realism. We further propose diversity rewards that encourage the model to generate planning behaviors that may not be present in logged driving data. Notably, our closed-loop training framework is scalable and does not require external simulators, which can be computationally expensive to run and have limited visual fidelity to the real-world. MAPLE achieves state-of-the-art driving performance on Bench2Drive and demonstrates scalable, closed-loop multi-agent play for robust E2E autonomous driving systems.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[vla]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.14201v2)
