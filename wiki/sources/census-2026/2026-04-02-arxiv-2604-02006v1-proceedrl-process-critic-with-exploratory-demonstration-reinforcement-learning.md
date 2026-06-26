---
type: source
source_type: arxiv
title: "ProCeedRL: Process Critic with Exploratory Demonstration Reinforcement Learning for LLM Agentic Reasoning"
authors: Jingyue Gao, Yanjiang Guo, Xiaoshuai Chen, Jianyu Chen
url: https://arxiv.org/abs/2604.02006v1
date: 2026-04-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [embodied-agents, agent-reliability, agentic-rl, agent-memory, arxiv, auto-ingested]
---

# ProCeedRL: Process Critic with Exploratory Demonstration Reinforcement Learning for LLM Agentic Reasoning

**arXiv:** [2604.02006v1](https://arxiv.org/abs/2604.02006v1) · 2026-04-02 · cs.AI
**Authors:** Jingyue Gao, Yanjiang Guo, Xiaoshuai Chen, Jianyu Chen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement Learning (RL) significantly enhances the reasoning abilities of large language models (LLMs), yet applying it to multi-turn agentic tasks remains challenging due to the long-horizon nature of interactions and the stochasticity of environmental feedback. We identify a structural failure mode in agentic exploration: suboptimal actions elicit noisy observations into misleading contexts, which further weaken subsequent decision-making, making recovery increasingly difficult. This cumulative feedback loop of errors renders standard exploration strategies ineffective and susceptible to the model's reasoning and the environment's randomness. To mitigate this issue, we propose ProCeedRL: Process Critic with Explorative Demonstration RL, shifting exploration from passive selection to active intervention. ProCeedRL employs a process-level critic to monitor interactions in real time, incorporating reflection-based demonstrations to guide agents in stopping the accumulation of errors. We find that this approach significantly exceeds the model's saturated exploration performance, demonstrating substantial exploratory benefits. By learning from exploratory demonstrations and on-policy samples, ProCeedRL significantly improves exploration efficiency and achieves superior performance on complex deep search and embodied tasks.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.02006v1)
