---
type: source
source_type: arxiv
title: "KD-MARL: Resource-Aware Knowledge Distillation in Multi-Agent Reinforcement Learning"
authors: Monirul Islam Pavel, Siyi Hu, Muhammad Anwar Masum, Mahardhika Pratama et al.
url: https://arxiv.org/abs/2604.06691v1
date: 2026-04-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# KD-MARL: Resource-Aware Knowledge Distillation in Multi-Agent Reinforcement Learning

**arXiv:** [2604.06691v1](https://arxiv.org/abs/2604.06691v1) · 2026-04-08 · cs.AI
**Authors:** Monirul Islam Pavel, Siyi Hu, Muhammad Anwar Masum, Mahardhika Pratama et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Real world deployment of multi agent reinforcement learning MARL systems is fundamentally constrained by limited compute memory and inference time. While expert policies achieve high performance they rely on costly decision cycles and large scale models that are impractical for edge devices or embedded platforms. Knowledge distillation KD offers a promising path toward resource aware execution but existing KD methods in MARL focus narrowly on action imitation often neglecting coordination structure and assuming uniform agent capabilities. We propose resource aware Knowledge Distillation for Multi Agent Reinforcement Learning KD MARL a two stage framework that transfers coordinated behavior from a centralized expert to lightweight decentralized student agents. The student policies are trained without a critic relying instead on distilled advantage signals and structured policy supervision to preserve coordination under heterogeneous and limited observations. Our approach transfers both action level behavior and structural coordination patterns from expert policies while supporting heterogeneous student architectures allowing each agent model capacity to match its observation complexity which is crucial for efficient execution under partial or limited observability and limited onboard resources. Extensive experiments on SMAC and MPE benchmarks demonstrate that KD MARL achieves high performance retention while substantially reducing computational cost. Across standard multi agent benchmarks KD MARL retains over 90 percent of expert performance while reducing computational cost by up to 28.6 times FLOPs. The proposed approach achieves expert level coordination and preserves it through structured distillation enabling practical MARL deployment across resource constrained onboard platforms.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.06691v1)
