---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentPRM: Process Reward Models for LLM Agents via Step-Wise Promise and Progress"
authors: Zhiheng Xi, Chenyang Liao, Guanyu Li, Yajie Yang et al.
url: https://arxiv.org/abs/2511.08325v1
date: 2025-11-11
citationCount: 35
influentialCitationCount: 2
velocity: 4.78
ingested: 2026-06-22
tags: [embodied-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# AgentPRM: Process Reward Models for LLM Agents via Step-Wise Promise and Progress

**arXiv [2511.08325v1](https://arxiv.org/abs/2511.08325v1)** · 2025-11-11 · **35 citations** (2 influential · 4.78/mo) · Zhiheng Xi, Chenyang Liao, Guanyu Li, Yajie Yang et al.

## Abstract
Despite rapid development, large language models (LLMs) still encounter challenges in multi-turn decision-making tasks (i.e., agent tasks) like web shopping and browser navigation, which require making a sequence of intelligent decisions based on environmental feedback. Previous work for LLM agents typically relies on elaborate prompt engineering or fine-tuning with expert trajectories to improve performance. In this work, we take a different perspective: we explore constructing process reward models (PRMs) to evaluate each decision and guide the agent's decision-making process. Unlike LLM reasoning, where each step is scored based on correctness, actions in agent tasks do not have a clear-cut correctness. Instead, they should be evaluated based on their proximity to the goal and the progress they have made. Building on this insight, we propose a re-defined PRM for agent tasks, named AgentPRM, to capture both the interdependence between sequential decisions and their contribution to the final goal. This enables better progress tracking and exploration-exploitation balance. To scalably obtain labeled data for training AgentPRM, we employ a Temporal Difference-based (TD-based) estimation method combined with Generalized Advantage Estimation (GAE), which proves more sample-efficient than prior methods. Extensive experiments across different agentic tasks show that AgentPRM is over $8\times$ more compute-efficient than baselines, and it demonstrates robust improvement when scaling up test-time compute. Moreover, we perform detailed analyses to show how our method works and offer more insights, e.g., applying AgentPRM to the reinforcement learning of LLM agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary and Background 2.0.0.1 Outcome Reward Model (ORM) 2.0.0.2 Process Reward Model (PRM) 2.0.0.3 Best-of-N (BoN) with reward models 2.0.0.4 Search with process reward models 3 Methodology 3.1 Motivation 3.2 AgentPRM: Re-Defining Process Rewards for LLM Agents 3.2.1 Measuring expected future success probability with value functions. 3.2.2 Capturing dependencies between steps with advantages. 3.3 Practical Implementation for Training AgentPRM 3.3.1 MC-based estimation 3.3.2 TD-based estimation with GAE 4 Experiments 4.1 Experimental Setup 4.1.1 Tasks. 4.1.2 Baselines. 4.1.3 Implementation Details. 4.1.4 Evaluation Settings. 4.2 Main Results 4.2.0.1 Result 1: Compared to greedy decoding, introducing RMs for BoN and search can improve LM performance on agent tasks. 4.2.0.2 Result 2: AgentPRM is more compute-efficient than other reward models, and outperforms them consistently in both Best-of-N and test-time search. 4.2.0.3 Result 3: As inference compute scaling, AgentPRM demonstrates a more robust a…

**Method / approach.** Methodology 3.1 Motivation 3.2 AgentPRM: Re-Defining Process Rewards for LLM Agents 3.2.1 Measuring expected future success probability with value functions. 3.2.2 Capturing dependencies between steps with advantages. 3.3 Practical Implementation for Training AgentPRM 3.3.1 MC-based estimation 3.3.2 TD-based estimation with GAE 4 Experiments 4.1 Experimental Setup 4.1.1 Tasks. 4.1.2 Baselines. 4.1.3 Implementation Details. 4.1.4 Evaluation Settings. 4.2 Main Results 4.2.0.1 Result 1: Compared to greedy decoding, introducing RMs for BoN and search can improve LM performance on agent tasks. 4.2.0.2 Result 2: AgentPRM is more compute-efficient than other reward models, and outperforms them consistently in both Best-of-N and test-time search. 4.2.0.3 Result 3: As inference compute scaling, AgentPRM demonstrates a more robust and stable scaling trend. 5 Discussion and Analysis 5.1 Ablation Study on ℒ A ​ ( ϕ ) \mathcal{L}_{A}(\phi)…

**Results.** Experiments 4.1 Experimental Setup 4.1.1 Tasks. 4.1.2 Baselines. 4.1.3 Implementation Details. 4.1.4 Evaluation Settings. 4.2 Main Results 4.2.0.1 Result 1: Compared to greedy decoding, introducing RMs for BoN and search can improve LM performance on agent tasks. 4.2.0.2 Result 2: AgentPRM is more compute-efficient than other reward models, and outperforms them consistently in both Best-of-N and test-time search. 4.2.0.3 Result 3: As inference compute scaling, AgentPRM demonstrates a more robust and stable scaling trend. 5 Discussion and Analysis 5.1 Ablation Study on ℒ A ​ ( ϕ ) \mathcal{L}_{A}(\phi) 5.2 Applying AgentPRM to Reinforcement Learning 5.3 Performance on Mathematical Reasoning 5.4 Comparing Sampling Efficiency of Our Method with MC-based Estimation 5.5 Evaluating Value Distributions of Actions with AgentPRM 5.6 Experiments on Models of Larger Size and Different Series 6 Related Wo…

**Conclusion.** Conclusion A More Detailed Discussion of Related Work B Algorithm C More Implementation Details for RL D Qualitative Analysis AgentPRM: Process Reward Models for LLM Agents via Step-Wise Promise and Progress Zhiheng Xi 1 ∗† Chenyang Liao 1 ∗ Guanyu Li 1 Yajie Yang 1 Wenxiang Chen 1 Zhihao Zhang 1 , Binghai Wang 1 , Senjie Jin 1 , Yuhao Zhou 1 , Jian Guan 2 , Wei Wu 2 , Tao Ji 1 , Tao Gui 1 † , Qi Zhang 1 † , Xuanjing Huang 1 † 1 Fudan University 2 Ant Group zhxi22@m.fudan.edu.cn, {tgui,xjhuang}@fudan.edu.cn Abstract Despite rapid development, large language models (LLMs) still encounter challenges in multi-turn decision-making tasks (i.e., agent tasks) like web shopping and browser navigation, which re…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.08325v1.md` · `raw/arxiv/2511.08325v1.fulltext.md`
