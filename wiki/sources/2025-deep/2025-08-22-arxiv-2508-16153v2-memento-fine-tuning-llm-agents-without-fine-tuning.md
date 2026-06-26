---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memento: Fine-tuning LLM Agents without Fine-tuning LLMs"
authors: Huichi Zhou, Yihang Chen, Siyuan Guo, Xue Yan et al.
url: https://arxiv.org/abs/2508.16153v2
date: 2025-08-22
citationCount: 71
influentialCitationCount: 6
velocity: 7.11
ingested: 2026-06-22
tags: [agentic-rl, agent-skills, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Memento: Fine-tuning LLM Agents without Fine-tuning LLMs

**arXiv [2508.16153v2](https://arxiv.org/abs/2508.16153v2)** · 2025-08-22 · **71 citations** (6 influential · 7.11/mo) · Huichi Zhou, Yihang Chen, Siyuan Guo, Xue Yan et al.

## Abstract
In this paper, we introduce a novel learning paradigm for Adaptive Large Language Model (LLM) agents that eliminates the need for fine-tuning the underlying LLMs. Existing approaches are often either rigid, relying on static, handcrafted reflection workflows, or computationally intensive, requiring gradient updates of LLM model parameters. In contrast, our method enables low-cost continual adaptation via memory-based online reinforcement learning. We formalise this as a Memory-augmented Markov Decision Process (M-MDP), equipped with a neural case-selection policy to guide action decisions. Past experiences are stored in an episodic memory, either differentiable or non-parametric. The policy is continually updated based on environmental feedback through a memory rewriting mechanism, whereas policy improvement is achieved through efficient memory reading (retrieval). We instantiate our agent model in the deep research setting, namely \emph{Memento}, which attains top-1 on GAIA validation ($87.88\%$ Pass@$3$) and $79.40\%$ on the test set. It reaches $66.6\%$ F1 and $80.4\%$ PM on the DeepResearcher dataset, outperforming the state-of-the-art training-based method, while case-based memory adds $4.7\%$ to $9.6\%$ absolute points on out-of-distribution tasks. Our approach offers a scalable and efficient pathway for developing generalist LLM agents capable of continuous, real-time learning without gradient updates, advancing machine learning towards open-ended skill acquisition and deep research scenarios. The code is available at https://github.com/Agent-on-the-Fly/Memento.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Continual-learning in LLM Agent Systems 2.2 Tool-augmented LLM 2.3 Agent Memory Mechanism 3 Methodology: Memory-Based MDP with Case-based Reasoning Policy Soft Q-Learning for CBR Agent. Enhance Q-Learning Based on State Similarity. 4 Implementation: Deep Research Agent 4.1 Framework 4.2 Case Memory Management 4.3 Tool Usage 5 Experiments 5.1 Datasets 5.2 Evaluation Metrics 5.3 Model Configurations 5.4 Experimental Results 5.5 Ablation Studies 5.5.1 Hyper-parameter Selection 5.5.2 Component-wise Analysis 5.5.3 Continual Learning Ability Boosted by Parametric and Non-Parametric CBR 5.5.4 Generalisation across Tasks 6 Discussion and Analysis 6.1 The Number of Tokens per Task 6.2 Statistics of MCP Tools 6.3 The Impact of Fast and Slow Think Mode 7 Conclusion A Derivation of the Optimal Policy in Soft-Q Learning B Analysis of Memory Mechanisms \correspondingauthor Linyi Yang: yangly6@sustech.edu.cn, and Jun Wang: jun.wang@cs.ucl.ac.uk Memento: Fine-tuning LLM Agents without…

**Method / approach.** Methodology: Memory-Based MDP with Case-based Reasoning Policy Soft Q-Learning for CBR Agent. Enhance Q-Learning Based on State Similarity. 4 Implementation: Deep Research Agent 4.1 Framework 4.2 Case Memory Management 4.3 Tool Usage 5 Experiments 5.1 Datasets 5.2 Evaluation Metrics 5.3 Model Configurations 5.4 Experimental Results 5.5 Ablation Studies 5.5.1 Hyper-parameter Selection 5.5.2 Component-wise Analysis 5.5.3 Continual Learning Ability Boosted by Parametric and Non-Parametric CBR 5.5.4 Generalisation across Tasks 6 Discussion and Analysis 6.1 The Number of Tokens per Task 6.2 Statistics of MCP Tools 6.3 The Impact of Fast and Slow Think Mode 7 Conclusion A Derivation of the Optimal Policy in Soft-Q Learning B Analysis of Memory Mechanisms \correspondingauthor Linyi Yang: yangly6@sustech.edu.cn, and Jun Wang: jun.wang@cs.ucl.ac.uk Memento: Fine-tuning LLM Agents without Fine-tuning LLMs Huichi Zhou AI…

**Results.** Experiments 5.1 Datasets 5.2 Evaluation Metrics 5.3 Model Configurations 5.4 Experimental Results 5.5 Ablation Studies 5.5.1 Hyper-parameter Selection 5.5.2 Component-wise Analysis 5.5.3 Continual Learning Ability Boosted by Parametric and Non-Parametric CBR 5.5.4 Generalisation across Tasks 6 Discussion and Analysis 6.1 The Number of Tokens per Task 6.2 Statistics of MCP Tools 6.3 The Impact of Fast and Slow Think Mode 7 Conclusion A Derivation of the Optimal Policy in Soft-Q Learning B Analysis of Memory Mechanisms \correspondingauthor Linyi Yang: yangly6@sustech.edu.cn, and Jun Wang: jun.wang@cs.ucl.ac.uk Memento: Fine-tuning LLM Agents without Fine-tuning LLMs Huichi Zhou AI Centre, UCL Huawei Noah’s Ark Lab, UK Yihang Chen Huawei Noah’s Ark Lab, UK Siyuan Guo Jilin University Xue Yan Institute of Automation, CAS Kin Hei Lee Zihan Wang Ka Yiu Lee Huaw…

**Conclusion.** Conclusion A Derivation of the Optimal Policy in Soft-Q Learning B Analysis of Memory Mechanisms \correspondingauthor Linyi Yang: yangly6@sustech.edu.cn, and Jun Wang: jun.wang@cs.ucl.ac.uk Memento: Fine-tuning LLM Agents without Fine-tuning LLMs Huichi Zhou AI Centre, UCL Huawei Noah’s Ark Lab, UK Yihang Chen Huawei Noah’s Ark Lab, UK Siyuan Guo Jilin University Xue Yan Institute of Automation, CAS Kin Hei Lee Zihan Wang Ka Yiu Lee Huawei Noah’s Ark Lab, UK Guchun Zhang Huawei Noah’s Ark Lab, UK Kun Shao Huawei Noah’s Ark Lab, UK Linyi Yang Huawei Noah’s Ark Lab, UK Jun Wang AI Centre, UCL Abstract Abstract In this paper, we introduce a novel learning paradigm for A…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2508.16153v2.md` · `raw/arxiv/2508.16153v2.fulltext.md`
