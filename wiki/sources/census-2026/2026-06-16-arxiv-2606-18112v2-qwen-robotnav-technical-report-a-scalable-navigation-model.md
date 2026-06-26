---
type: source
source_type: arxiv
title: "Qwen-RobotNav Technical Report: A Scalable Navigation Model Designed for an Agentic Navigation System"
authors: Jiazhao Zhang, Gengze Zhou, Hale Yin, Yiyang Huang et al.
url: https://arxiv.org/abs/2606.18112v2
date: 2026-06-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.RO
tags: [autonomous-driving-agents, embodied-agents, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Qwen-RobotNav Technical Report: A Scalable Navigation Model Designed for an Agentic Navigation System

**arXiv:** [2606.18112v2](https://arxiv.org/abs/2606.18112v2) · 2026-06-16 · cs.RO
**Authors:** Jiazhao Zhang, Gengze Zhou, Hale Yin, Yiyang Huang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic navigation systems require a base navigation model whose observation strategy can be externally reconfigured at inference time, because instruction following, object search, target tracking, and autonomous driving share the same perception-planning backbone yet demand fundamentally different strategies for consuming the visual stream. We present Qwen-RobotNav, a scalable navigation model built on Qwen-RobotNav that addresses it through a parameterised interface with two complementary dimensions: multiple task modes that select the navigation behaviour, and controllable observation parameters (e.g., token budget, per-camera weights) that govern how visual history is encoded. With training-time randomization over all parameters, Qwen-RobotNav is robust to any inference-time configuration requiring zero architectural modification to the Qwen-RobotNav backbone. We train Qwen-RobotNav on 15.6M samples; co-training with vision-language data prevents the collapse into reactive action-sequence mappers observed in trajectory-only training. The parameterised interface also makes Qwen-RobotNav a natural building block for agentic systems: for long-horizon scenarios, an upper-level planner decomposes goals into sub-tasks and dynamically switches Qwen-RobotNav's task mode and context strategy mid-episode, composing complex behaviours from repeated calls to the same model. Extensive experiments show that Qwen-RobotNav sets new state-of-the-art results across major navigation benchmarks. The model exhibits favourable scaling from 2B to 8B parameters, with joint multi-task training developing a shared spatial-planning substrate that transfers across task families, and demonstrates strong zero-shot generalisation to real-world robots across diverse environments.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.18112v2)
