---
type: source
source_type: arxiv
title: "MagicAgent: Towards Generalized Agent Planning"
authors: Xuhui Ren, Shaokang Dong, Chen Yang, Qing Gao et al.
url: https://arxiv.org/abs/2602.19000v2
date: 2026-02-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MagicAgent: Towards Generalized Agent Planning

**arXiv:** [2602.19000v2](https://arxiv.org/abs/2602.19000v2) · 2026-02-22 · cs.AI
**Authors:** Xuhui Ren, Shaokang Dong, Chen Yang, Qing Gao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The evolution of Large Language Models (LLMs) from passive text processors to autonomous agents has established planning as a core component of modern intelligence. However, achieving generalized planning remains elusive, not only by the scarcity of high-quality interaction data but also by inherent conflicts across heterogeneous planning tasks. These challenges result in models that excel at isolated tasks yet struggle to generalize, while existing multi-task training attempts suffer from gradient interference. In this paper, we present \textbf{MagicAgent}, a series of foundation models specifically designed for generalized agent planning. We introduce a lightweight and scalable synthetic data framework that generates high-quality trajectories across diverse planning tasks, including hierarchical task decomposition, tool-augmented planning, multi-constraint scheduling, procedural logic orchestration, and long-horizon tool execution. To mitigate training conflicts, we propose a two-stage training paradigm comprising supervised fine-tuning followed by multi-objective reinforcement learning over both static datasets and dynamic environments. Empirical results show that MagicAgent-32B and MagicAgent-30B-A3B achieve superior performance across diverse open-source benchmarks (\emph{e.g.}, $75.1\%$ on Worfbench and $86.9\%$ on BFCL-v3), as well as strong results on our in-house MagicEval benchmarks, substantially outperforming existing sub-100B models and surpassing leading ultra-scale models, including GPT-5.2, Kimi-K2 and GLM-4.7.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.19000v2)
