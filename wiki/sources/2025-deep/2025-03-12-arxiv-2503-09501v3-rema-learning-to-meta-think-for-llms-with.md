---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ReMA: Learning to Meta-think for LLMs with Multi-Agent Reinforcement Learning"
authors: Ziyu Wan, Yunxiang Li, Xiaoyu Wen, Yan Song et al.
url: https://arxiv.org/abs/2503.09501v3
date: 2025-03-12
citationCount: 66
influentialCitationCount: 4
velocity: 4.3
ingested: 2026-06-22
tags: [human-agent-interaction, agent-reliability, agentic-rl, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# ReMA: Learning to Meta-think for LLMs with Multi-Agent Reinforcement Learning

**arXiv [2503.09501v3](https://arxiv.org/abs/2503.09501v3)** · 2025-03-12 · **66 citations** (4 influential · 4.3/mo) · Ziyu Wan, Yunxiang Li, Xiaoyu Wen, Yan Song et al.

## Abstract
Recent research on Reasoning of Large Language Models (LLMs) has sought to further enhance their performance by integrating meta-thinking -- enabling models to monitor, evaluate, and control their reasoning processes for more adaptive and effective problem-solving. However, current single-agent work lacks a specialized design for acquiring meta-thinking, resulting in low efficacy. To address this challenge, we introduce Reinforced Meta-thinking Agents (ReMA), a novel framework that leverages Multi-Agent Reinforcement Learning (MARL) to elicit meta-thinking behaviors, encouraging LLMs to think about thinking. ReMA decouples the reasoning process into two hierarchical agents: a high-level meta-thinking agent responsible for generating strategic oversight and plans, and a low-level reasoning agent for detailed executions. Through iterative reinforcement learning with aligned objectives, these agents explore and learn collaboration, leading to improved generalization and robustness. Empirical results from single-turn experiments demonstrate that ReMA outperforms single-agent RL baselines on complex reasoning tasks, including competitive-level mathematical benchmarks and LLM-as-a-Judge benchmarks. Additionally, we further extend ReMA to multi-turn interaction settings, leveraging turn-level ratio and parameter sharing to improve efficiency. Comprehensive ablation studies further illustrate the evolving dynamics of each distinct agent, providing valuable insights into how the meta-thinking reasoning process enhances the reasoning capabilities of LLMs. Our code can be found in https://github.com/ziyuwan/ReMA-public

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 2.1 Vanilla Reasoning Process (VRP) 2.2 Training VRP via Reinforcement Learning 3 Method 3.1 Deploying Meta-Thinking Reasoning Process for LLMs 3.2 Training MAMRP: A Multi-Agent RL Method 3.2.1 Optimizing Single-turn MAMRP 3.2.2 Scaling up to Multi-turn MAMRP 4 Experiments 4.1 Experiment Settings Benchmarks Baselines, Models, Training Settings 4.2 Results of Single-turn ReMA 4.2.1 Meta-thoughts boost low-level generalization 4.2.2 Diverse meta-thinking characteristics of LLMs 4.3 Extending ReMA to Multi-turn MAMRP 4.3.1 Results and Ablations 5 Conclusion A Related work A.1 Single LLM Reasoning A.2 Multiple LLM Reasoning A.3 Hierarchical Reasoning A.4 RL in LLM B Limitation and Future Work C Supplementary Materials for Method in Section 3 C.1 Inference-time Scaling of ReMA C.2 Detailed reward design 1. Correctness and Format-Aware Reward (Base Setting) 2. Consistency-Based Reward C.3 Pseudocode of ReMA C.4 Brief convergence analysis C.5 Learning to reason…

**Method / approach.** Method 3.1 Deploying Meta-Thinking Reasoning Process for LLMs 3.2 Training MAMRP: A Multi-Agent RL Method 3.2.1 Optimizing Single-turn MAMRP 3.2.2 Scaling up to Multi-turn MAMRP 4 Experiments 4.1 Experiment Settings Benchmarks Baselines, Models, Training Settings 4.2 Results of Single-turn ReMA 4.2.1 Meta-thoughts boost low-level generalization 4.2.2 Diverse meta-thinking characteristics of LLMs 4.3 Extending ReMA to Multi-turn MAMRP 4.3.1 Results and Ablations 5 Conclusion A Related work A.1 Single LLM Reasoning A.2 Multiple LLM Reasoning A.3 Hierarchical Reasoning A.4 RL in LLM B Limitation and Future Work C Supplementary Materials for Method in Section 3 C.1 Inference-time Scaling of ReMA C.2 Detailed reward design 1. Correctness and Format-Aware Reward (Base Setting) 2. Consistency-Based Reward C.3 Pseudocode of ReMA C.4 Brief convergence analysis C.5 Learning to reason from the perspective o…

**Results.** Experiments 4.1 Experiment Settings Benchmarks Baselines, Models, Training Settings 4.2 Results of Single-turn ReMA 4.2.1 Meta-thoughts boost low-level generalization 4.2.2 Diverse meta-thinking characteristics of LLMs 4.3 Extending ReMA to Multi-turn MAMRP 4.3.1 Results and Ablations 5 Conclusion A Related work A.1 Single LLM Reasoning A.2 Multiple LLM Reasoning A.3 Hierarchical Reasoning A.4 RL in LLM B Limitation and Future Work C Supplementary Materials for Method in Section 3 C.1 Inference-time Scaling of ReMA C.2 Detailed reward design 1. Correctness and Format-Aware Reward (Base Setting) 2. Consistency-Based Reward C.3 Pseudocode of ReMA C.4 Brief convergence analysis C.5 Learning to reason from the perspective of Leader Follower Game C.5.1 Leader-follower game C.5.2 Efficacy of LLM C.5.3 Leader-follower Game for LLM Reasoning D Training Details…

**Conclusion.** Conclusion A Related work A.1 Single LLM Reasoning A.2 Multiple LLM Reasoning A.3 Hierarchical Reasoning A.4 RL in LLM B Limitation and Future Work C Supplementary Materials for Method in Section 3 C.1 Inference-time Scaling of ReMA C.2 Detailed reward design 1. Correctness and Format-Aware Reward (Base Setting) 2. Consistency-Based Reward C.3 Pseudocode of ReMA C.4 Brief convergence analysis C.5 Learning to reason from the perspective of Leader Follower Game C.5.1 Leader-follower game C.5.2 Efficacy of LLM C.5.3 Leader-follower Game for LLM Reasoning D Training Details D.1 Single-turn ReMA D.1.1 Supervised fine-tuning data collection D.1.2 Dataset Curation of RewardBench970…

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2503.09501v3.md` · `raw/arxiv/2503.09501v3.fulltext.md`
