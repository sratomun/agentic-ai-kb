---
type: source
source_type: arxiv
title: "CoRe-Code: Collaborative Reinforcement Learning for Code Generation"
authors: Zhihao Dou, Qinjian Zhao, Zhongwei Wan, Xiaoyu Xia et al.
url: https://arxiv.org/abs/2605.24812v1
date: 2026-05-24
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# CoRe-Code: Collaborative Reinforcement Learning for Code Generation

**arXiv:** [2605.24812v1](https://arxiv.org/abs/2605.24812v1) · 2026-05-24 · cs.AI
**Authors:** Zhihao Dou, Qinjian Zhao, Zhongwei Wan, Xiaoyu Xia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) have achieved strong performance in code generation, but most methods rely on autoregressive decoding without global planning, often leading to locally coherent yet globally suboptimal solutions (e.g., failing test cases or inefficient complexity). While recent approaches such as Chain-of-Thought (CoT) and multi-agent systems (MAS) introduce planning, their limited role specialization and coordination hinder performance on complex tasks. To address the challenges of coordination and specialization in multi-agent code generation, we propose Collaborative Reinforcement Code (CoRe-Code), a framework for role specialized LLM agents that enhances inter-agent coordination to generate more accurate and efficient code. CoRe-Code adopts a simple Planner-Coder paradigm, where the Planner produces high-level plans and the Coder executes them to generate code. We further introduce a collaboration-aware reinforcement learning stage based on Group Relative Policy Optimization (GRPO) to enhance role specialization and alignment. Experiments show that CoRe-Code outperforms a wide range of existing RL-based and multi-agent methods. In addition, we demonstrate that CoRe-Code can generalize to other multi-agent frameworks (e.g., Retrieval and Debugging agents), highlighting its flexibility and scalability. We evaluate CoRe-Code on multiple benchmarks of varying difficulty using three base models. Compared to existing baselines, the results show consistent improvements in accuracy, while also achieving higher efficiency in terms of execution time and memory usage, demonstrating the effectiveness and practicality of CoRe-Code.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.24812v1)
