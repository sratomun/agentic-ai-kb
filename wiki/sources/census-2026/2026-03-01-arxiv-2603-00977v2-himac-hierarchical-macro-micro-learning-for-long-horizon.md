---
type: source
source_type: arxiv
title: "HiMAC: Hierarchical Macro-Micro Learning for Long-Horizon LLM Agents"
authors: Hongbo Jin, Rongpeng Zhu, Jiayu Ding, Guibo Luo et al.
url: https://arxiv.org/abs/2603.00977v2
date: 2026-03-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# HiMAC: Hierarchical Macro-Micro Learning for Long-Horizon LLM Agents

**arXiv:** [2603.00977v2](https://arxiv.org/abs/2603.00977v2) · 2026-03-01 · cs.AI
**Authors:** Hongbo Jin, Rongpeng Zhu, Jiayu Ding, Guibo Luo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) agents have recently demonstrated strong capabilities in interactive decision-making, yet they remain fundamentally limited in long-horizon tasks that require structured planning and reliable execution. Existing approaches predominantly rely on flat autoregressive policies, where high-level reasoning and low-level actions are generated within a single token sequence, leading to inefficient exploration and severe error propagation over extended trajectories. In this work, we propose HiMAC, a hierarchical agentic RL framework that explicitly decomposes long-horizon decision-making into macro-level planning and micro-level execution. HiMAC models reasoning as a structured blueprint generation process followed by goal-conditioned action execution, enabling robust long-horizon planning within LLM-based agents. To train this hierarchy efficiently, we introduce a critic-free hierarchical policy optimization paradigm that extends group-based reinforcement learning to bi-level structures through hierarchical relative advantage estimation. Furthermore, we propose an iterative co-evolution training strategy that alternates between planner exploration and executor adaptation, mitigating the non-stationarity inherent in hierarchical learning. Extensive experiments on ALFWorld, WebShop, and Sokoban demonstrate that HiMAC consistently outperforms strong prompting and reinforcement learning baselines, achieving state-of-the-art performance and substantially improved sample efficiency across both text-based and visually grounded environments. Our results show that introducing structured hierarchy, rather than increasing model scale alone, is a key factor for enabling robust long-horizon agentic intelligence.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Entities:** [[alfworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00977v2)
