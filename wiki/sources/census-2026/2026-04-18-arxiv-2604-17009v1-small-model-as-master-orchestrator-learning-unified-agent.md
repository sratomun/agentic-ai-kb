---
type: source
source_type: arxiv
title: "Small Model as Master Orchestrator: Learning Unified Agent-Tool Orchestration with Parallel Subtask Decomposition"
authors: Wenzhen Yuan, Wutao Xiong, Fanchen Yu, Shengji Tang et al.
url: https://arxiv.org/abs/2604.17009v1
date: 2026-04-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Small Model as Master Orchestrator: Learning Unified Agent-Tool Orchestration with Parallel Subtask Decomposition

**arXiv:** [2604.17009v1](https://arxiv.org/abs/2604.17009v1) · 2026-04-18 · cs.AI
**Authors:** Wenzhen Yuan, Wutao Xiong, Fanchen Yu, Shengji Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent systems (MAS) demonstrate clear advantages in tackling complex problems by coordinating diverse agents and external tools. However, most existing orchestration methods rely on static workflows or serial agent scheduling, and are further constrained by heterogeneous interface protocols between tools and agents. This leads to high system complexity and poor extensibility. To mitigate these issues, we propose Agent-as-Tool, a unified parallel orchestration paradigm that abstracts both agents and tools into a standardized, learnable action space with protocol normalization and explicit state feedback. Building on this paradigm, we train a lightweight orchestrator, ParaManager, which decouples planning decisions from subtask solving, enabling state-aware parallel subtask decomposition, delegation, and asynchronous execution. For training, we adopt a two-stage ParaManager training pipeline. It improves robustness by incorporating supervised fine-tuning (SFT) trajectories equipped with recovery mechanisms, and further applies reinforcement learning (RL) to achieve an optimal balance among task success, protocol compliance, diversity, and reasoning efficiency. Experiments show that ParaManager achieves strong performance across multiple benchmarks and exhibits robust generalization under unseen model pools.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17009v1)
