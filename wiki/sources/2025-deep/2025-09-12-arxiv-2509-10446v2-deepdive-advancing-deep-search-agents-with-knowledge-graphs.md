---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepDive: Advancing Deep Search Agents with Knowledge Graphs and Multi-Turn RL"
authors: Rui Lu, Zhenyu Hou, Zihan Wang, Hanchen Zhang et al.
url: https://arxiv.org/abs/2509.10446v2
date: 2025-09-12
citationCount: 38
influentialCitationCount: 10
velocity: 4.09
ingested: 2026-06-22
tags: [computer-use-agents, knowledge-graph, agentic-rl, agent-memory, tool-use, arxiv, 2025, cited]
---

# DeepDive: Advancing Deep Search Agents with Knowledge Graphs and Multi-Turn RL

**arXiv [2509.10446v2](https://arxiv.org/abs/2509.10446v2)** · 2025-09-12 · **38 citations** (10 influential · 4.09/mo) · Rui Lu, Zhenyu Hou, Zihan Wang, Hanchen Zhang et al.

## Abstract
Augmenting large language models (LLMs) with browsing tools substantially improves their potential as deep search agents to solve complex, real-world tasks. Yet, open LLMs still perform poorly in such settings due to limited long-horizon reasoning capacity with browsing tools and the lack of sufficiently difficult supervised data. To address these challenges, we present DeepDive to advance deep search agents. First, we propose a strategy to automatically synthesize complex, difficult, and hard-to-find questions from open knowledge graphs. Second, we apply end-to-end multi-turn reinforcement learning (RL) to enhance LLMs' long-horizon reasoning with deep search. To encourage diversity and reduce redundancy, we design a redundancy penalty that discourages repeated similar queries. Experiments show that DeepDive-32B achieves a new open-source competitive result on BrowseComp, outperforming WebSailor, DeepSeek-R1-Browse, and Search-o1. We demonstrate that multi-turn RL training improves deep search ability and significantly contributes to the performance improvements across multiple benchmarks. We observe that DeepDive enables test-time scaling of tool calls and parallel sampling. All datasets, models, and code are publicly available at https://github.com/THUDM/DeepDive.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 The DeepDive Method 2.1 Automated Data Synthesis from Knowledge Graphs Knowledge Graphs with Hard-to-Find Information. Automated Data Synthesis from KGs. Improving Path Quality and Complexity. 2.2 End-to-End Multi-Turn Reinforcement Learning Multi-Turn RL. Encouraging Diverse Search with Redundancy Penalty. 3 Experiments 3.1 Setup Benchmarks. Baselines. Data Synthesis Details. Training Details. Evaluation. 3.2 Overall Performance Competitive among Open Deep Search Agents. RL Drives Deeper Search Strategies. 3.3 Test-Time Scaling for DeepDive Tool Call Scaling during Inference. Parallel Sampling and Tool Call Voting. 3.4 Ablation Study Reward Ablation. Synthetic Data Ablation. 4 Additional Study: Semi-Automated i.i.d. Deep Search QA Synthesis for RL i.i.d. Data Synthesis. RL with i.i.d. Deep Search Data. Data Contamination Analysis. 5 Related Work Reinforcement Learning for LLMs. Deep Search Agents. 6 Conclusion 7 Limitation A Generalization on Simple Search Tasks B Case…

**Method / approach.** Method 2.1 Automated Data Synthesis from Knowledge Graphs Knowledge Graphs with Hard-to-Find Information. Automated Data Synthesis from KGs. Improving Path Quality and Complexity. 2.2 End-to-End Multi-Turn Reinforcement Learning Multi-Turn RL. Encouraging Diverse Search with Redundancy Penalty. 3 Experiments 3.1 Setup Benchmarks. Baselines. Data Synthesis Details. Training Details. Evaluation. 3.2 Overall Performance Competitive among Open Deep Search Agents. RL Drives Deeper Search Strategies. 3.3 Test-Time Scaling for DeepDive Tool Call Scaling during Inference. Parallel Sampling and Tool Call Voting. 3.4 Ablation Study Reward Ablation. Synthetic Data Ablation. 4 Additional Study: Semi-Automated i.i.d. Deep Search QA Synthesis for RL i.i.d. Data Synthesis. RL with i.i.d. Deep Search Data. Data Contamination Analysis. 5 Related Work Reinforcement Learning for LLMs. Deep Search Agents. 6 Conclusion…

**Results.** Experiments 3.1 Setup Benchmarks. Baselines. Data Synthesis Details. Training Details. Evaluation. 3.2 Overall Performance Competitive among Open Deep Search Agents. RL Drives Deeper Search Strategies. 3.3 Test-Time Scaling for DeepDive Tool Call Scaling during Inference. Parallel Sampling and Tool Call Voting. 3.4 Ablation Study Reward Ablation. Synthetic Data Ablation. 4 Additional Study: Semi-Automated i.i.d. Deep Search QA Synthesis for RL i.i.d. Data Synthesis. RL with i.i.d. Deep Search Data. Data Contamination Analysis. 5 Related Work Reinforcement Learning for LLMs. Deep Search Agents. 6 Conclusion 7 Limitation A Generalization on Simple Search Tasks B Case Study Reinforcement Learning Reshapes the Model’s Search Strategy DeepDive: Advancing Deep Search Agents with Knowledge Graphs and Multi-Turn RL Rui Lu 12∗† , Zhenyu Hou 12∗ , Zihan Wang 23∗† ,…

**Conclusion.** Conclusion 7 Limitation A Generalization on Simple Search Tasks B Case Study Reinforcement Learning Reshapes the Model’s Search Strategy DeepDive: Advancing Deep Search Agents with Knowledge Graphs and Multi-Turn RL Rui Lu 12∗† , Zhenyu Hou 12∗ , Zihan Wang 23∗† , Hanchen Zhang 1† , Xiao Liu 12 , Yujiang Li 1† , Shi Feng 3 , Jie Tang 1 , Yuxiao Dong 1 1 Tsinghua University 2 Z.AI 3 Northeastern University {learningrate1, zhenyu.hou08, wzh1998921}@gmail.com Abstract Augmenting large language models (LLMs) with browsing tools substantially improves their potential as deep search agents to solve complex, real-world tasks. Yet, open LLMs still perform poorly in such settings due to limited long-horizon reasoni…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[deepseek]]
- **Raw:** `raw/arxiv/2509.10446v2.md` · `raw/arxiv/2509.10446v2.fulltext.md`
