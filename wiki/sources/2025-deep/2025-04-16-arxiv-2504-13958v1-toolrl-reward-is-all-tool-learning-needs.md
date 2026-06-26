---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ToolRL: Reward is All Tool Learning Needs"
authors: Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang et al.
url: https://arxiv.org/abs/2504.13958v1
date: 2025-04-16
citationCount: 280
influentialCitationCount: 35
velocity: 19.73
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# ToolRL: Reward is All Tool Learning Needs

**arXiv [2504.13958v1](https://arxiv.org/abs/2504.13958v1)** · 2025-04-16 · **280 citations** (35 influential · 19.73/mo) · Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang et al.

## Abstract
Current Large Language Models (LLMs) often undergo supervised fine-tuning (SFT) to acquire tool use capabilities. However, SFT struggles to generalize to unfamiliar or complex tool use scenarios. Recent advancements in reinforcement learning (RL), particularly with R1-like models, have demonstrated promising reasoning and generalization abilities. Yet, reward design for tool use presents unique challenges: multiple tools may be invoked with diverse parameters, and coarse-grained reward signals, such as answer matching, fail to offer the finegrained feedback required for effective learning. In this work, we present the first comprehensive study on reward design for tool selection and application tasks within the RL paradigm. We systematically explore a wide range of reward strategies, analyzing their types, scales, granularity, and temporal dynamics. Building on these insights, we propose a principled reward design tailored for tool use tasks and apply it to train LLMs using Group Relative Policy Optimization (GRPO). Empirical evaluations across diverse benchmarks demonstrate that our approach yields robust, scalable, and stable training, achieving a 17% improvement over base models and a 15% gain over SFT models. These results highlight the critical role of thoughtful reward design in enhancing the tool use capabilities and generalization performance of LLMs. All the codes are released to facilitate future research.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Tool-Integrated Reasoning of LLMs. Exploration of RL in LLMs. 3 Method 3.1 Task Definition 3.2 TIR Rollout 3.3 Reward Design Format Reward. Correctness Reward. 3.4 RL Training with GRPO Normalized Advantage Across Query Groups. Policy Optimization Objective. 4 Experiments 4.1 Training Dataset 4.2 Experiment Settings Training. Evaluation. Baselines. 4.3 Results Main Results. SFT Initialization Impacts. Reward Design on PPO. Generalization Studies. Free-form Inference Effectiveness. 5 Analysis 5.1 Effect of Length Reward Dynamic Length Reward. 5.2 Effect of Reward Scale Dynamic Reward Scaling. 5.3 Effect of Reward Granularity 6 Conclusion A User Prompt Details B Experiment Details Training Data Details. GRPO Setting Details. Baselines. PPO Setting Details. C Additional Results ToolRL: Reward is All Tool Learning Needs Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang, Xiusi Chen, Dilek Hakkani-Tür, Gokhan Tur, Heng Ji University of Illinois…

**Method / approach.** Method 3.1 Task Definition 3.2 TIR Rollout 3.3 Reward Design Format Reward. Correctness Reward. 3.4 RL Training with GRPO Normalized Advantage Across Query Groups. Policy Optimization Objective. 4 Experiments 4.1 Training Dataset 4.2 Experiment Settings Training. Evaluation. Baselines. 4.3 Results Main Results. SFT Initialization Impacts. Reward Design on PPO. Generalization Studies. Free-form Inference Effectiveness. 5 Analysis 5.1 Effect of Length Reward Dynamic Length Reward. 5.2 Effect of Reward Scale Dynamic Reward Scaling. 5.3 Effect of Reward Granularity 6 Conclusion A User Prompt Details B Experiment Details Training Data Details. GRPO Setting Details. Baselines. PPO Setting Details. C Additional Results ToolRL: Reward is All Tool Learning Needs Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang, Xiusi Chen, Dilek Hakkani-Tür, Gokhan Tur, Heng Ji University of Illinois Urb…

**Results.** Experiments 4.1 Training Dataset 4.2 Experiment Settings Training. Evaluation. Baselines. 4.3 Results Main Results. SFT Initialization Impacts. Reward Design on PPO. Generalization Studies. Free-form Inference Effectiveness. 5 Analysis 5.1 Effect of Length Reward Dynamic Length Reward. 5.2 Effect of Reward Scale Dynamic Reward Scaling. 5.3 Effect of Reward Granularity 6 Conclusion A User Prompt Details B Experiment Details Training Data Details. GRPO Setting Details. Baselines. PPO Setting Details. C Additional Results ToolRL: Reward is All Tool Learning Needs Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang, Xiusi Chen, Dilek Hakkani-Tür, Gokhan Tur, Heng Ji University of Illinois Urbana-Champaign {chengq9, hengji}@illinois.edu Abstract Current Large Language Models (LLMs) often undergo supervised fine-tuning (SFT) to acquire tool use capabilities. How…

**Conclusion.** Conclusion A User Prompt Details B Experiment Details Training Data Details. GRPO Setting Details. Baselines. PPO Setting Details. C Additional Results ToolRL: Reward is All Tool Learning Needs Cheng Qian, Emre Can Acikgoz, Qi He, Hongru Wang, Xiusi Chen, Dilek Hakkani-Tür, Gokhan Tur, Heng Ji University of Illinois Urbana-Champaign {chengq9, hengji}@illinois.edu Abstract Current Large Language Models (LLMs) often undergo supervised fine-tuning (SFT) to acquire tool use capabilities. However, SFT struggles to generalize to unfamiliar or complex tool use scenarios. Recent advancements in reinforcement learning (RL), particularly with R1-like models, have demonstrated promising reasoning and generalization abili…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2504.13958v1.md` · `raw/arxiv/2504.13958v1.fulltext.md`
