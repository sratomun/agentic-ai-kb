---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent-R: Training Language Model Agents to Reflect via Iterative Self-Training"
authors: Siyu Yuan, Zehui Chen, Zhiheng Xi, Junjie Ye et al.
url: https://arxiv.org/abs/2501.11425v3
date: 2025-01-20
citationCount: 56
influentialCitationCount: 3
velocity: 3.29
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Agent-R: Training Language Model Agents to Reflect via Iterative Self-Training

**arXiv [2501.11425v3](https://arxiv.org/abs/2501.11425v3)** · 2025-01-20 · **56 citations** (3 influential · 3.29/mo) · Siyu Yuan, Zehui Chen, Zhiheng Xi, Junjie Ye et al.

## Abstract
Large Language Models (LLMs) agents are increasingly pivotal for addressing complex tasks in interactive environments. Existing work mainly focuses on enhancing performance through behavior cloning from stronger experts, yet such approaches often falter in real-world applications, mainly due to the inability to recover from errors. However, step-level critique data is difficult and expensive to collect. Automating and dynamically constructing self-critique datasets is thus crucial to empowering models with intelligent agent capabilities. In this work, we propose an iterative self-training framework, Agent-R, that enables language Agent to Reflect on the fly. Unlike traditional methods that reward or penalize actions based on correctness, Agent-R leverages MCTS to construct training data that recover correct trajectories from erroneous ones. A key challenge of agent reflection lies in the necessity for timely revision rather than waiting until the end of a rollout. To address this, we introduce a model-guided critique construction mechanism: the actor model identifies the first error step (within its current capability) in a failed trajectory. Starting from it, we splice it with the adjacent correct path, which shares the same parent node in the tree. This strategy enables the model to learn reflection based on its current policy, therefore yielding better learning efficiency. To further explore the scalability of this self-improvement paradigm, we investigate iterative refinement of both error correction capabilities and dataset construction. Our findings demonstrate that Agent-R continuously improves the model's ability to recover from errors and enables timely error correction. Experiments on three interactive environments show that Agent-R effectively equips agents to correct erroneous actions while avoiding loops, achieving superior performance compared to baseline methods (+5.59%).

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary 2.1 Task Formulation 2.2 Monte Carlo Tree Search 3 Method 3.1 Phase I: Model-Guided Reflection Trajectory Generation Reflection Trajectory Definition Trajectory Collection with MCTS Transition Point Determination with Actor Model 3.2 Phase II: Iterative Self-Training with Revision Trajectories 4 Experiment 4.1 Interactive and Agentic Environments 4.2 Experiment Setting Data Split MCTS Settings Training Settings Baselines Evaluation Metrics 4.3 Main Result 4.4 Findings with Analysis Finding 1: Training with trajectories from Agent-R can outperform using optimal trajectories. Finding 2: Agent-R can effectively provide language agents with self-reflection capabilities. Finding 3: Training with revision trajectories helps agents more easily identify and correct erroneous actions. Finding 4: Training with revision trajectories helps agents avoid getting stuck in loops. Finding 5: Multi-task training is a more effective strategy for Agent-R. 5 Related Work Agent Learning in Interactive…

**Method / approach.** Method 3.1 Phase I: Model-Guided Reflection Trajectory Generation Reflection Trajectory Definition Trajectory Collection with MCTS Transition Point Determination with Actor Model 3.2 Phase II: Iterative Self-Training with Revision Trajectories 4 Experiment 4.1 Interactive and Agentic Environments 4.2 Experiment Setting Data Split MCTS Settings Training Settings Baselines Evaluation Metrics 4.3 Main Result 4.4 Findings with Analysis Finding 1: Training with trajectories from Agent-R can outperform using optimal trajectories. Finding 2: Agent-R can effectively provide language agents with self-reflection capabilities. Finding 3: Training with revision trajectories helps agents more easily identify and correct erroneous actions. Finding 4: Training with revision trajectories helps agents avoid getting stuck in loops. Finding 5: Multi-task training is a more effective strategy for Agent-R. 5 Related Work Agent Learning in I…

**Results.** Experiment 4.1 Interactive and Agentic Environments 4.2 Experiment Setting Data Split MCTS Settings Training Settings Baselines Evaluation Metrics 4.3 Main Result 4.4 Findings with Analysis Finding 1: Training with trajectories from Agent-R can outperform using optimal trajectories. Finding 2: Agent-R can effectively provide language agents with self-reflection capabilities. Finding 3: Training with revision trajectories helps agents more easily identify and correct erroneous actions. Finding 4: Training with revision trajectories helps agents avoid getting stuck in loops. Finding 5: Multi-task training is a more effective strategy for Agent-R. 5 Related Work Agent Learning in Interactive Environments Self-Correction for Large Language Models 6 Conclusion 7 Prompt Template of Revision Trajectory 8 Trajectory Definition 9 Experiment Details 9.1 Training and Evaluation D…

**Conclusion.** Conclusion 7 Prompt Template of Revision Trajectory 8 Trajectory Definition 9 Experiment Details 9.1 Training and Evaluation Details 9.2 Multi-task training v.s. Single-task Training 9.3 Case Study Error Correction in Trajectory Generation Adaptive Transition Point Evaluation 1]Fudan University 2]ByteDance Seed \contribution [*]Equal contributions \contribution [†]Work done at ByteDance Seed Agent-R \xspace : Training Language Model Agents to Reflect via Iterative Self-Training Siyu Yuan Zehui Chen Zhiheng Xi Junjie Ye Zhengyin Du Jiecao Chen [ [ syyuan21@m.fudan.edu.cn (March 24, 2025) Abstract Large Language Models (LLMs) agents are increasingly pivotal for addressing compl…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2501.11425v3.md` · `raw/arxiv/2501.11425v3.fulltext.md`
