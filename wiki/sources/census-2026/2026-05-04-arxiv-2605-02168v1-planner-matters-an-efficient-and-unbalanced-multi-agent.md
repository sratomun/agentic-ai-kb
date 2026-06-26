---
type: source
source_type: arxiv
title: "Planner Matters! An Efficient and Unbalanced Multi-agent Collaboration Framework for Long-horizon Planning"
authors: Wenyi Wu, Sibo Zhu, Kun Zhou, Biwei Huang
url: https://arxiv.org/abs/2605.02168v1
date: 2026-05-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [computer-use-agents, embodied-agents, agentic-rl, agent-memory, tool-use, arxiv, auto-ingested]
---

# Planner Matters! An Efficient and Unbalanced Multi-agent Collaboration Framework for Long-horizon Planning

**arXiv:** [2605.02168v1](https://arxiv.org/abs/2605.02168v1) · 2026-05-04 · cs.AI
**Authors:** Wenyi Wu, Sibo Zhu, Kun Zhou, Biwei Huang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Language model (LM)-based agents have demonstrated promising capabilities in automating complex tasks from natural language instructions, yet they continue to struggle with long-horizon planning and reasoning. To address this, we propose an enhanced multi-agent framework that decomposes automation into three roles: a planner for high-level decision-making, an actor for task execution, and a memory manager for contextual reasoning. While this modular decomposition aligns with established design patterns, our core contribution lies in a systematic compute-allocation analysis, revealing that planning is the dominant factor influencing task performance. Execution and memory management require significantly less compute and model capacity to achieve competitive results. Building on these insights, we introduce a planner-centric reinforcement learning approach, which exclusively optimizes the planner using trajectory-level rewards from a VLM-as-judge, while freezing the other components. Extensive experiments on benchmarks spanning web navigation, OS control, and tool use demonstrate that concentrating model capacity and learning on high-level planning yields robust and compute-efficient improvements in long-horizon agent automation. Our code is publicly released.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02168v1)
