---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Chain-of-Agents: End-to-End Agent Foundation Models via Multi-Agent Distillation and Agentic RL"
authors: Weizhen Li, Jianbo Lin, Zhuosong Jiang, Jingyi Cao et al.
url: https://arxiv.org/abs/2508.13167v1
date: 2025-08-06
citationCount: 62
influentialCitationCount: 8
velocity: 5.9
ingested: 2026-06-22
tags: [coding-agents, computer-use-agents, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# Chain-of-Agents: End-to-End Agent Foundation Models via Multi-Agent Distillation and Agentic RL

**arXiv [2508.13167v1](https://arxiv.org/abs/2508.13167v1)** · 2025-08-06 · **62 citations** (8 influential · 5.9/mo) · Weizhen Li, Jianbo Lin, Zhuosong Jiang, Jingyi Cao et al.

## Abstract
Recent advances in large language models (LLMs) and multi-agent systems have demonstrated remarkable capabilities in complex problem-solving tasks such as deep research, vibe coding, and mathematical reasoning. However, most existing multi-agent systems are built upon manual prompt/workflow engineering with sophisticated agent frameworks, making them computationally inefficient, less capable, and can not benefit from data-centric learning. In this work, we introduce Chain-of-Agents (CoA), a novel paradigm of LLM reasoning that enables native end-to-end complex problem-solving in the same way as a multi-agent system (i.e., multi-turn problem solving with multiple tools and multiple agents) within one model. In chain-of-agents problem-solving, the model dynamically activates different tool agents and role-playing agents to simulate multi-agent collaboration in an end-to-end fashion. To elicit end-to-end chain-of-agents problem-solving abilities in LLMs, we introduce a multi-agent distillation framework to distill state-of-the-art multi-agent systems into chain-of-agents trajectories for agentic supervised fine-tuning. We then use agentic reinforcement learning on verifiable agentic tasks to further improve the models' capabilities on chain-of-agents problem solving. We call the resulting models Agent Foundation Models (AFMs). Our empirical studies demonstrate that AFM establishes new state-of-the-art performance across diverse benchmarks in both web agent and code agent settings. We make the entire research, including the model weights, code for training and evaluation, and the training data, fully open-sourced, which offers a solid starting point for future research on agent models and agentic RL.

## From the paper (full-text excerpts)
**Introduction.** Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2 Background . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 Method . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 4 4 Chain-of-Agents Paradigm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4 3.2 Agentic Supervised Fine-tuning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.2.1 Training Data Generation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5 5 3.3 Agentic Reinforcement Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.3.1 Data Sampling for RL Training . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.3.2 Reward Function Design . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8 8 8 4 Experiments . . . . . . . . . . . . . .…

**Method / approach.** methods on GAIA, BrowseComp, HLE, and AIME25 benchmarks. AFM demonstrates consistent effectiveness across web agent and code agent benchmarks. 1 Contents 1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2 Background . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 Method . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 4 4 Chain-of-Agents Paradigm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4 3.2 Agentic Supervised Fine-tuning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.2.1 Training Data Generation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5 5 3.3 Agentic Reinforcement Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3.3.1 D…

**Results.** Experiments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9 4.1 Web Agent Experiments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4.1.1 Experimental Setup . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4.1.2 Experimental Results . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9 9 13 Code Agent Experiments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4.2.1 Experimental Setup . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4.2.2 Experimental Results . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14 14 16 3.1 4.2 5 Analysis . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17…

**Conclusion.** Conclusion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 21 8 Contributions . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 22 Appendix . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 28 2 1 Introduction Recent advances in multi-agent systems (MAS) [2, 6, 44, 46, 53, 80–83] have demonstrated remarkable capabilities in complex problem-solving tasks such as deep research and vibe coding. These multi-agent frameworks enable complex problem-solving via collaboration between multiple agents with diverse roles and tool sets. Despite their impressive performance…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2508.13167v1.md` · `raw/arxiv/2508.13167v1.fulltext.md`
