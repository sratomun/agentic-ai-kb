---
type: source
source_type: arxiv
title: "AgenticQwen: Training Small Agentic Language Models with Dual Data Flywheels for Industrial-Scale Tool Use"
authors: Yuanjie Lyu, Chengyu Wang, Haonan Zheng, Yuanhao Yue et al.
url: https://arxiv.org/abs/2604.21590v1
date: 2026-04-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# AgenticQwen: Training Small Agentic Language Models with Dual Data Flywheels for Industrial-Scale Tool Use

**arXiv:** [2604.21590v1](https://arxiv.org/abs/2604.21590v1) · 2026-04-23 · cs.CL
**Authors:** Yuanjie Lyu, Chengyu Wang, Haonan Zheng, Yuanhao Yue et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Modern industrial applications increasingly demand language models that act as agents, capable of multi-step reasoning and tool use in real-world settings. These tasks are typically performed under strict cost and latency constraints, making small agentic models highly desirable. In this paper, we introduce the AgenticQwen family of models, trained via multi-round reinforcement learning (RL) on synthetic data and a limited amount of open-source data. Our training framework combines reasoning RL and agentic RL with dual data flywheels that automatically generate increasingly challenging tasks. The reasoning flywheel increases task difficulty by learning from errors, while the agentic flywheel expands linear workflows into multi-branch behavior trees that better reflect the decision complexity of real-world applications. We validate AgenticQwen on public benchmarks and in an industrial agent system. The models achieve strong performance on multiple agentic benchmarks, and in our industrial agent system, close the gap with much larger models on search and data analysis tasks. Model checkpoints and part of the synthetic data: https://huggingface.co/collections/alibaba-pai/agenticqwen. Data synthesis and RL training code: https://github.com/haruhi-sudo/data_synth_and_rl. The data synthesis pipeline is also integrated into EasyDistill: https://github.com/modelscope/easydistill.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.21590v1)
