---
type: source
source_type: arxiv
title: "Learning Rollout from Sampling:An R1-Style Tokenized Traffic Simulation Model"
authors: Ziyan Wang, Peng Chen, Ding Li, Chiwei Li et al.
url: https://arxiv.org/abs/2603.24989v1
date: 2026-03-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.RO
tags: [autonomous-driving-agents, agentic-rl, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Learning Rollout from Sampling:An R1-Style Tokenized Traffic Simulation Model

**arXiv:** [2603.24989v1](https://arxiv.org/abs/2603.24989v1) · 2026-03-26 · cs.RO
**Authors:** Ziyan Wang, Peng Chen, Ding Li, Chiwei Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Learning diverse and high-fidelity traffic simulations from human driving demonstrations is crucial for autonomous driving evaluation. The recent next-token prediction (NTP) paradigm, widely adopted in large language models (LLMs), has been applied to traffic simulation and achieves iterative improvements via supervised fine-tuning (SFT). However, such methods limit active exploration of potentially valuable motion tokens, particularly in suboptimal regions. Entropy patterns provide a promising perspective for enabling exploration driven by motion token uncertainty. Motivated by this insight, we propose a novel tokenized traffic simulation policy, R1Sim, which represents an initial attempt to explore reinforcement learning based on motion token entropy patterns, and systematically analyzes the impact of different motion tokens on simulation outcomes. Specifically, we introduce an entropy-guided adaptive sampling mechanism that focuses on previously overlooked motion tokens with high uncertainty yet high potential. We further optimize motion behaviors using Group Relative Policy Optimization (GRPO), guided by a safety-aware reward design. Overall, these components enable a balanced exploration-exploitation trade-off through diverse high-uncertainty sampling and group-wise comparative estimation, resulting in realistic, safe, and diverse multi-agent behaviors. Extensive experiments on the Waymo Sim Agent benchmark demonstrate that R1Sim achieves competitive performance compared to state-of-the-art methods.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.24989v1)
