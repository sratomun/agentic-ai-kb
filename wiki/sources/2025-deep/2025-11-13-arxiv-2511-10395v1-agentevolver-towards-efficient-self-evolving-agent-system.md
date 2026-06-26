---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "AgentEvolver: Towards Efficient Self-Evolving Agent System"
authors: Yunpeng Zhai, Shuchang Tao, Cheng Chen, Anni Zou et al.
url: https://arxiv.org/abs/2511.10395v1
date: 2025-11-13
citationCount: 44
influentialCitationCount: 4
velocity: 6.06
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# AgentEvolver: Towards Efficient Self-Evolving Agent System

**arXiv [2511.10395v1](https://arxiv.org/abs/2511.10395v1)** · 2025-11-13 · **44 citations** (4 influential · 6.06/mo) · Yunpeng Zhai, Shuchang Tao, Cheng Chen, Anni Zou et al.

## Abstract
Autonomous agents powered by large language models (LLMs) have the potential to significantly enhance human productivity by reasoning, using tools, and executing complex tasks in diverse environments. However, current approaches to developing such agents remain costly and inefficient, as they typically require manually constructed task datasets and reinforcement learning (RL) pipelines with extensive random exploration. These limitations lead to prohibitively high data-construction costs, low exploration efficiency, and poor sample utilization. To address these challenges, we present AgentEvolver, a self-evolving agent system that leverages the semantic understanding and reasoning capabilities of LLMs to drive autonomous agent learning. AgentEvolver introduces three synergistic mechanisms: (i) self-questioning, which enables curiosity-driven task generation in novel environments, reducing dependence on handcrafted datasets; (ii) self-navigating, which improves exploration efficiency through experience reuse and hybrid policy guidance; and (iii) self-attributing, which enhances sample efficiency by assigning differentiated rewards to trajectory states and actions based on their contribution. By integrating these mechanisms into a unified framework, AgentEvolver enables scalable, cost-effective, and continual improvement of agent capabilities. Preliminary experiments indicate that AgentEvolver achieves more efficient exploration, better sample utilization, and faster adaptation compared to traditional RL-based baselines.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Problem Formulation Environment Formulation Target Task Space and Oracle Reward Proxy Objective of Self-Evolution 3 Self-Questioning 3.1 Curiosity-Guided Exploration with Environment Profiles Environment Profiles as Action Priors LLM-Driven Stochastic Exploration 3.2 Adaptive Task Synthesis Preference Guided Task Synthesis Reference Solution Extraction 3.3 Task Curation and Distributional Hybrid Real-time Filtering Post-generation Filtering Distributional Hybrid (Optional) 3.4 Synthetic Task Reward with LLM Judge LLM as a Judge Basic Principle Reference-based Correctness Check 4 Self-Navigating Notion of Experience 4.1 Experience Acquisition Pool Construction Experience Retrieval 4.2 Experience-mixed Rollout Trajectory Generation Advantage Computation 4.3 Experience Incorporation Experience Stripping Selective Boosting 5 Self-Attributing 5.1 Step-wise Attribution via LLM-based Reasoning 5.2 Attribution-Based Reward Construction Quantification of Attribution Labels.…

**Method / approach.** methods for LLM-based agents suffer from severe sample inefficiency. Although the RL community has proposed various exploration strategies such as intrinsic rewards ( DBLP:journals/corr/abs-2502-01456 ) and UCB-based bandit methods ( song2025outcome ) , these techniques are often ineffective for long-horizon, tool-augmented agents, where each rollout is computationally and financially expensive. As a result, current LLM agent training still primarily adopts PPO- or GRPO-style policy optimization ( deepseek_math ) , whose reliance on massive trajectory sampling leads to approximate brute-force exploration with many redundant rollouts and limited learning value. Consequently, the training of LLM agents remains a laborious and costly paradigm. Motivated by the rapidly growing semantic understanding and reasoning capabilities of LLMs, a natural question arises: why not entrust the model itself with greater autonomy in driving its own learning process? Instead of relying on rigid, hu…

**Results.** Experiments 7.1 Experimental Settings 7.1.1 Benchmarks and Evaluations 7.1.2 Baselines and Backbone Models 7.1.3 Implementation Details Self-Questioning Self-Navigating Self-Attributing 7.2 Main Results 7.3 Results of Self-Questioning 7.3.1 Effectiveness of Synthetic Data 7.3.2 Influence of Synthetic Data Quantity 7.3.3 Capability Generalization with Synthetic Data 7.3.4 Ablation Study on the LLM Judge 7.4 Results of Self-Navigating 7.4.1 Effectiveness of Experience on Navigation 7.4.2 Implicit vs. Explicit Experience Learning 7.4.3 Exploration vs. Exploitation Dynamics 7.4.4 Short-term vs. Long-term Optimization 7.5 Results of Self-Attributing 7.5.1 Effectiveness of Self-Attributing 7.5.2 Sample Efficiency of Self-Attributing 7.5.3 Hyperparameter Analysis 7.6 Effectiveness of Context-Managing Templates 8 Conclusion and Next Steps 1. Challenge-oriented applications.…

**Conclusion.** Conclusion and Next Steps 1. Challenge-oriented applications. 2. Scaling to larger models. 3. LLM-level self-evolving. AgentEvolver : Towards Efficient Self-Evolving Agent System Yunpeng Zhai 1 1 footnotemark: 1 , Shuchang Tao 1 1 footnotemark: 1 , Cheng Chen 1 1 footnotemark: 1 , Anni Zou 1 1 footnotemark: 1 , Ziqian Chen 1 1 footnotemark: 1 , Qingxu Fu 1 1 footnotemark: 1 , Shinji Mai 1 1 footnotemark: 1 , Li Yu, Jiaji Deng, Zouying Cao, Zhaoyang Liu 2 2 footnotemark: 2 , Bolin Ding 2 2 footnotemark: 2 , Jingren Zhou Tongyi Lab , Alibaba Group {zhaiyunpeng.zyp, taoshuchang.tsc, chengchen, zouanni.zan, eric.czq, fuqingxu.fqx, jingmu.lzy, bolin.ding}@alibaba-inc.com Abstract Autonomous agents powere…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2511.10395v1.md` · `raw/arxiv/2511.10395v1.fulltext.md`
