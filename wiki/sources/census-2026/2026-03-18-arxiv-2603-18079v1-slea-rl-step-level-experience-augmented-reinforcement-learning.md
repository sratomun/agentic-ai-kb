---
type: source
source_type: arxiv
title: "SLEA-RL: Step-Level Experience Augmented Reinforcement Learning for Multi-Turn Agentic Training"
authors: Prince Zizhuang Wang, Shuli Jiang
url: https://arxiv.org/abs/2603.18079v1
date: 2026-03-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.LG
tags: [self-evolving-agents, agentic-rl, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# SLEA-RL: Step-Level Experience Augmented Reinforcement Learning for Multi-Turn Agentic Training

**arXiv:** [2603.18079v1](https://arxiv.org/abs/2603.18079v1) · 2026-03-18 · cs.LG
**Authors:** Prince Zizhuang Wang, Shuli Jiang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) agents have shown strong results on multi-turn tool-use tasks, yet they operate in isolation during training, failing to leverage experiences accumulated across episodes. Existing experience-augmented methods address this by organizing trajectories into retrievable libraries, but they retrieve experiences only once based on the initial task description and hold them constant throughout the episode. In multi-turn settings where observations change at every step, this static retrieval becomes increasingly mismatched as episodes progress. We propose SLEA-RL (Step-Level Experience-Augmented Reinforcement Learning), a framework that retrieves relevant experiences at each decision step conditioned on the current observation. SLEA-RL operates through three components: (i) step-level observation clustering that groups structurally equivalent environmental states for efficient cluster-indexed retrieval; (ii) a self-evolving experience library that distills successful strategies and failure patterns through score-based admission and rate-limited extraction; and (iii) policy optimization with step-level credit assignment for fine-grained advantage estimation across multi-turn episodes. The experience library evolves alongside the policy through semantic analysis rather than gradient updates. Experiments on long-horizon multi-turn agent benchmarks demonstrate that SLEA-RL achieves superior performance compared to various reinforcement learning baselines.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.18079v1)
