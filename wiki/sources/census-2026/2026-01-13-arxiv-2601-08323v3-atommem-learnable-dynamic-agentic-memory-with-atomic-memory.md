---
type: source
source_type: arxiv
title: "AtomMem : Learnable Dynamic Agentic Memory with Atomic Memory Operation"
authors: Yupeng Huo, Yaxi Lu, Zhong Zhang, Haotian Chen et al.
url: https://arxiv.org/abs/2601.08323v3
date: 2026-01-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AtomMem : Learnable Dynamic Agentic Memory with Atomic Memory Operation

**arXiv:** [2601.08323v3](https://arxiv.org/abs/2601.08323v3) · 2026-01-13 · cs.AI
**Authors:** Yupeng Huo, Yaxi Lu, Zhong Zhang, Haotian Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Equipping agents with memory is essential for solving real-world long-horizon problems. However, most existing agent memory mechanisms rely on static and hand-crafted workflows. This limits the performance and generalization ability of these memory designs, which highlights the need for a more flexible, learning-based memory framework. In this paper, we propose AtomMem, which reframes memory management as a dynamic decision-making problem. We deconstruct high-level memory processes into fundamental atomic CRUD (Create, Read, Update, Delete) operations, transforming the memory workflow into a learnable decision process. By combining supervised fine-tuning with reinforcement learning, AtomMem learns an autonomous, task-aligned policy to orchestrate memory behaviors tailored to specific task demands. Experimental results across 3 long-context benchmarks demonstrate that the trained AtomMem-8B consistently outperforms prior static-workflow memory methods. Further analysis of training dynamics shows that our learning-based formulation enables the agent to discover structured, task-aligned memory management strategies, highlighting a key advantage over predefined routines.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.08323v3)
