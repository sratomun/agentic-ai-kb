---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents"
authors: Zijian Zhou, Ao Qu, Zhaoxuan Wu, Sunghwan Kim et al.
url: https://arxiv.org/abs/2506.15841v2
date: 2025-06-18
citationCount: 150
influentialCitationCount: 13
velocity: 12.37
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, arxiv, 2025, cited]
---

# MEM1: Learning to Synergize Memory and Reasoning for Efficient Long-Horizon Agents

**arXiv [2506.15841v2](https://arxiv.org/abs/2506.15841v2)** · 2025-06-18 · **150 citations** (13 influential · 12.37/mo) · Zijian Zhou, Ao Qu, Zhaoxuan Wu, Sunghwan Kim et al.

## Abstract
Modern language agents must operate over long-horizon, multi-turn interactions, where they retrieve external information, adapt to observations, and answer interdependent queries. Yet, most LLM systems rely on full-context prompting, appending all past turns regardless of their relevance. This leads to unbounded memory growth, increased computational costs, and degraded reasoning performance on out-of-distribution input lengths. We introduce MEM1, an end-to-end reinforcement learning framework that enables agents to operate with constant memory across long multi-turn tasks. At each turn, MEM1 updates a compact shared internal state that jointly supports memory consolidation and reasoning. This state integrates prior memory with new observations from the environment while strategically discarding irrelevant or redundant information. To support training in more realistic and compositional settings, we propose a simple yet effective and scalable approach to constructing multi-turn environments by composing existing datasets into arbitrarily complex task sequences. Experiments across three domains, including internal retrieval QA, open-domain web QA, and multi-turn web shopping, show that MEM1-7B improves performance by 3.5x while reducing memory usage by 3.7x compared to Qwen2.5-14B-Instruct on a 16-objective multi-hop QA task, and generalizes beyond the training horizon. Our results demonstrate the promise of reasoning-driven memory consolidation as a scalable alternative to existing solutions for training long-horizon interactive agents, where both efficiency and performance are optimized.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work LLM agents in multi-turn environment. Memory management for LLM agents. 3 MEM1 3.1 Memory as Part of Reasoning 3.2 Masked Trajectory for Policy Optimization 3.3 Multi-Objective Task Design 4 Experiments Results 4.1 Implementation Details Datasets and evaluation metrics. Baselines. Meta info injection. 4.2 MEM1 on Multi-Objective Multi-Hop Tasks 4.3 MEM1 on Single-Objective Multi-Hop Tasks Long-horizon web navigation in WebShop. Single-objective QA in Wikipedia. Zero-shot transfer to Online Web-QA. 4.4 Analysis on Emergent Agent Behaviors 5 Conclusion, Limitations, and Future Work A Details of MEM1 A.1 Computing Resources and Training Details A.2 RAG Configuration A.3 Prompts A.4 Implementation Details of Metrics and Baselines A.4.1 Metrics Exact match. F1 score. Peak token usage. Dependency length. Inference time. A.4.2 Baselines Search-R1. Deep Researcher. A.5 Algorithm A.6 MEM1 on Webshop Training Details A.7 Additional Discussion on the Attention Matri…

**Method / approach.** method effectively scales up these tasks to enable long-horizon agent training. Motivated by this question, we present MEM1 : M emory- E fficient M echanism via learning 1 -step integrated reasoning and consolidation—a method for training LLM agents that maintain constant memory usage across arbitrarily long horizons. Figure 2 : A conceptual comparison of context length between the MEM1 agent and existing reasoning agents when handling long-horizon tasks. Our agent learns to discard the previous context (except for the prompt and initial query) immediately after generating a new internal state and action, resulting in near-constant memory usage. As illustrated in Fig. 1 , at each turn, the model updates a consolidated state composed of prior memory and newly obtained information. This consolidated state becomes the agent’s only retained memory, allowing all external tool outputs to be discarded after use, which prevents prompt expansion altogether as illustrated by Fig.…

**Results.** Experiments Results 4.1 Implementation Details Datasets and evaluation metrics. Baselines. Meta info injection. 4.2 MEM1 on Multi-Objective Multi-Hop Tasks 4.3 MEM1 on Single-Objective Multi-Hop Tasks Long-horizon web navigation in WebShop. Single-objective QA in Wikipedia. Zero-shot transfer to Online Web-QA. 4.4 Analysis on Emergent Agent Behaviors 5 Conclusion, Limitations, and Future Work A Details of MEM1 A.1 Computing Resources and Training Details A.2 RAG Configuration A.3 Prompts A.4 Implementation Details of Metrics and Baselines A.4.1 Metrics Exact match. F1 score. Peak token usage. Dependency length. Inference time. A.4.2 Baselines Search-R1. Deep Researcher. A.5 Algorithm A.6 MEM1 on Webshop Training Details A.7 Additional Discussion on the Attention Matrix Design. B Broader Impacts C Training Trajectory Analysis of MEM1 D Analysis on Imp…

**Conclusion.** Conclusion, Limitations, and Future Work A Details of MEM1 A.1 Computing Resources and Training Details A.2 RAG Configuration A.3 Prompts A.4 Implementation Details of Metrics and Baselines A.4.1 Metrics Exact match. F1 score. Peak token usage. Dependency length. Inference time. A.4.2 Baselines Search-R1. Deep Researcher. A.5 Algorithm A.6 MEM1 on Webshop Training Details A.7 Additional Discussion on the Attention Matrix Design. B Broader Impacts C Training Trajectory Analysis of MEM1 D Analysis on Implementation Details D.1 RL Generalizes Better Than SFT D.2 Format Reward Accelerates Convergence but Degrades Final Performance MEM1 : Learning to Synergize Memory and Reasoning…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2506.15841v2.md` · `raw/arxiv/2506.15841v2.fulltext.md`
