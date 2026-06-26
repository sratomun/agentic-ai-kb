---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "RAGEN: Understanding Self-Evolution in LLM Agents via Multi-Turn Reinforcement Learning"
authors: Zihan Wang, Kangrui Wang, Qineng Wang, Pingyue Zhang et al.
url: https://arxiv.org/abs/2504.20073v2
date: 2025-04-24
citationCount: 236
influentialCitationCount: 14
velocity: 16.94
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# RAGEN: Understanding Self-Evolution in LLM Agents via Multi-Turn Reinforcement Learning

**arXiv [2504.20073v2](https://arxiv.org/abs/2504.20073v2)** · 2025-04-24 · **236 citations** (14 influential · 16.94/mo) · Zihan Wang, Kangrui Wang, Qineng Wang, Pingyue Zhang et al.

## Abstract
Training large language models (LLMs) as interactive agents presents unique challenges including long-horizon decision making and interacting with stochastic environment feedback. While reinforcement learning (RL) has enabled progress in static tasks, multi-turn agent RL training remains underexplored. We propose StarPO (State-Thinking-Actions-Reward Policy Optimization), a general framework for trajectory-level agent RL, and introduce RAGEN, a modular system for training and evaluating LLM agents. Our study on four stylized environments reveals three core findings. First, our agent RL training shows a recurring mode of Echo Trap where reward variance cliffs and gradient spikes; we address this with StarPO-S, a stabilized variant with trajectory filtering, critic incorporation, and gradient stabilization. Second, we find the shaping of RL rollouts would benefit from diverse initial states, medium interaction granularity and more frequent sampling. Third, we show that without fine-grained, reasoning-aware reward signals, agent reasoning hardly emerge through multi-turn RL and they may show shallow strategies or hallucinated thoughts. Code and environments are available at https://github.com/RAGEN-AI/RAGEN.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Framework 2.1 The MDP Formulation for Agent Training 2.2 StarPO: Reinforcing Reasoning via Trajectory-Level Optimization 2.2.2 Optimization Procedure: Learning from Reasoning-Interaction Trajectories 2.2.3 Modular Optimization Strategies 2.3 The RAGEN System 3 Experiment Setup 3.1 Environments and Tasks 3.2 Training Settings 3.3 Evaluation Metrics 4 Experimental Results and Findings 4.1 Multi-turn Agent RL Training Introduces New Instability Pattern 4.2 StarPO-S: Stabilize Multi-turn RL with Instance Filtering and Gradient Shaping 4.3 Generating Useful Trajectories for RL Training 4.4 Reasoning Improves Generalization but Fades in Multi-Turn Settings Without Fine-Grained Rewards 5 Related Work 6 Conclusions and Limitations A Background of Reinforcement Learning B Extended Related Work C Detailed Experimental Settings C.1 Environments and Tasks Bi-Arm Bandits. C.2 Training and Evaluation Settings C.3 Evaluation Metrics D Results on Larger Models and Various Optimization Algorithms Scaling Effec…

**Method / approach.** methods focus on non-interactive tasks such as math or code generation. RAGEN implements StarPO, a general agent RL framework that supports multi-turn rollouts, trajectory-level reward assignment, and policy updates, on agent tasks requiring multi-turn stochastic interaction. 1 Introduction Training large language models (LLMs) to function as autonomous agents in interactive environments presents unique challenges. Unlike static tasks such as single-turn math problem solving (Shao et al., 2024a ) or coding (DeepSeek-AI et al., 2024 ) , agent settings require models to make sequential decisions, maintain memory across turns, and adapt to stochastic feedback from their environment. These settings—central to planning assistants, robotics, and tutoring agents—demand that models not only perform well, but also self-improve through experience. While recent work has explored reinforcement learning (RL) for LLMs (DeepSeek-AI et al., 2025 ; OpenAI, 2024 ; Pan et al., 2025 ; Zeng et…

**Results.** Experiment Setup 3.1 Environments and Tasks 3.2 Training Settings 3.3 Evaluation Metrics 4 Experimental Results and Findings 4.1 Multi-turn Agent RL Training Introduces New Instability Pattern 4.2 StarPO-S: Stabilize Multi-turn RL with Instance Filtering and Gradient Shaping 4.3 Generating Useful Trajectories for RL Training 4.4 Reasoning Improves Generalization but Fades in Multi-Turn Settings Without Fine-Grained Rewards 5 Related Work 6 Conclusions and Limitations A Background of Reinforcement Learning B Extended Related Work C Detailed Experimental Settings C.1 Environments and Tasks Bi-Arm Bandits. C.2 Training and Evaluation Settings C.3 Evaluation Metrics D Results on Larger Models and Various Optimization Algorithms Scaling Effects. Frontier Model Performance. Gradient Shaping. Response Masking and Bi-Level GAE. E When Does Uncertainty-Based Filtering Help? F Case S…

**Conclusion.** Conclusions and Limitations A Background of Reinforcement Learning B Extended Related Work C Detailed Experimental Settings C.1 Environments and Tasks Bi-Arm Bandits. C.2 Training and Evaluation Settings C.3 Evaluation Metrics D Results on Larger Models and Various Optimization Algorithms Scaling Effects. Frontier Model Performance. Gradient Shaping. Response Masking and Bi-Level GAE. E When Does Uncertainty-Based Filtering Help? F Case Study: The Emergence of Echo Trap with RL G Comparing Agent RL with Supervised Fine-Tuning H Efficient Training with Low-Rank Adaptation (LoRA) Motivation. I PPO Failure Mode in Frozen Lake J Prompt Templates J.1 Bi-Arm Bandit Environment Prompts J…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.20073v2.md` · `raw/arxiv/2504.20073v2.fulltext.md`
