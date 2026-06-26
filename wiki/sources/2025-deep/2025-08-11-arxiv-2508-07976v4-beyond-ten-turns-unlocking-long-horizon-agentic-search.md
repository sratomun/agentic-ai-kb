---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Beyond Ten Turns: Unlocking Long-Horizon Agentic Search with Large-Scale Asynchronous RL"
authors: Jiaxuan Gao, Wei Fu, Minyang Xie, Shusheng Xu et al.
url: https://arxiv.org/abs/2508.07976v4
date: 2025-08-11
citationCount: 117
influentialCitationCount: 37
velocity: 11.31
ingested: 2026-06-22
tags: [agent-memory, tool-use, agentic-ai, arxiv, 2025, cited]
---

# Beyond Ten Turns: Unlocking Long-Horizon Agentic Search with Large-Scale Asynchronous RL

**arXiv [2508.07976v4](https://arxiv.org/abs/2508.07976v4)** · 2025-08-11 · **117 citations** (37 influential · 11.31/mo) · Jiaxuan Gao, Wei Fu, Minyang Xie, Shusheng Xu et al.

## Abstract
Recent advancements in LLM-based agents have demonstrated remarkable capabilities in handling complex, knowledge-intensive tasks by integrating external tools. Among diverse choices of tools, search tools play a pivotal role in accessing vast external knowledge. However, open-source agents still fall short of achieving expert-level Search Intelligence, the ability to resolve ambiguous queries, generate precise searches, analyze results, and conduct thorough exploration. Existing approaches fall short in scalability, efficiency, and data quality. For example, small turn limits in existing online RL methods, e.g. <=10, restrict complex strategy learning. This paper introduces ASearcher, an open-source project for large-scale RL training of search agents. Our key contributions include: (1) Scalable fully asynchronous RL training that enables long-horizon search while maintaining high training efficiency. (2) A prompt-based LLM agent that autonomously synthesizes high-quality and challenging QAs, creating a large-scale QA dataset. Through RL training, our prompt-based QwQ-32B agent achieves substantial improvements, with 78.0% and 34.3% Avg@4 gains on xBench and GAIA, respectively. Notably, our agent exhibits extreme long-horizon search, with tool calls exceeding 100 turns and output tokens exceeding 400k during training time. With a simple agent design and no external LLMs, ASearcher-Web-QwQ achieves Avg@4 scores of 51.1 on xBench and 58.7 on GAIA, surpassing existing open-source 32B agents. Finally, we also show that ASearcher-Web-QwQ could achieve performance of commercial systems using external summary tool in a zero-shot transfer manner and test-time search. We open-source our models, training data, and codes in https://github.com/inclusionAI/ASearcher.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Limitations of Existing Open-source Approaches Solution Path of the Sample Question. Existing Online RL Approaches Fail to Learn Complex Search Strategies. Prompt-based LLM Agents Could Fail Due to Insufficient Capability of the LLM. ASearcher-Web-QwQ. 3 ASearcher 3.1 Agent Design Tools. Webpage Summarization. Instantiating ASearcher with Base LLMs and Advanced LRMs. End-to-End Reinforcement Learning. 3.2 Training Data 3.2.1 Open-source Data. 3.2.2 Data Synthesis Agent 3.3 Asynchronous Agentic RL Training 3.3.1 Challenges of Scaling Up Trajectory Length in RL Complex Tasks Require Long Trajectories. High Variance in Trajectory Execution Time. Efficiency Issues of Agentic RL Training. 3.3.2 Fully Asynchronous RL Training. Asynchronous Trajectory Rollouts. Decoupled Rollout and Training. 3.4 Training Details MDP Formulation. GRPO Training. Dynamic Filtering. Reward Function. 4 Experiments 4.1 Experiment Setup Benchmarks. Search Tools. Baselines Evaluation Metrics Training Details…

**Method / approach.** methods, e.g. ≤ 10 \leq 10 , restrict complex strategy learning. This paper introduces ASearcher, an open-source project for large-scale RL training of search agents. Our key contributions include: (1) Scalable fully asynchronous RL training that enables long-horizon search while maintaining high training efficiency. (2) A prompt-based LLM agent that autonomously synthesizes high-quality and challenging QAs. Through RL training, our prompt-based QwQ-32B agent achieves substantial improvements. Notably, our agent exhibits extreme long-horizon search, with tool calls exceeding 100 turns and output tokens exceeding 400k during training time. With a simple agent design and no external LLMs, ASearcher-Web-QwQ achieves Avg@4 scores of 51.1 on xBench and 58.7 on GAIA, surpassing existing open-source 32B agents. Finally, we also show that ASearcher-Web-QwQ could achieve performance of commercial systems using external summary tool in a zero-shot transfer manner and test-time search. 1 1 1 We…

**Results.** Experiments 4.1 Experiment Setup Benchmarks. Search Tools. Baselines Evaluation Metrics Training Details of ASearcher. Two-Stage Curriculum. 4.2 Main Results Local Knowledge Base with RAG on Standard QA Benchmarks. Web-based Search and Browsing on Standard QA Benchmarks Web-based Search and Browsing on Challenging Benchmarks. Effect of RL Training. Zero-Shot Transfer with Summary Tool Test-time Scaling. 4.3 Training Dynamics Training Dynamics of ASearcher-Local-7B/14B. Training Dynamics of ASearcher-Web-QwQ. 4.4 Emergent Behaviors Keyword Analysis. 5 Related Works Search Agents. Synthetic Data for Search Agents. 6 Conclusion A Full Case Study Solution Path of the Sample Question. Existing Online RL Approaches Fail to Learn Complex Search Strategies. Prompt-based LLM Agents Could Fail Due to Insufficient Capability of the LLM. ASearcher-Web-QwQ. Beyond Ten Turns…

**Conclusion.** Conclusion A Full Case Study Solution Path of the Sample Question. Existing Online RL Approaches Fail to Learn Complex Search Strategies. Prompt-based LLM Agents Could Fail Due to Insufficient Capability of the LLM. ASearcher-Web-QwQ. Beyond Ten Turns: Unlocking Long-Horizon Agentic Search with Large-Scale Asynchronous RL Jiaxuan Gao 1 , Wei Fu 12 , Minyang Xie 1 , Shusheng Xu 2 , Chuyi He 2 , Zhiyu Mei 2 , Banghua Zhu 3 , Yi Wu 1 1 IIIS, Tsinghua University, 2 Ant Group 3 University of Washington samjia2000@gmail.com , jxwuyi@gmail.com Corresponding author Abstract Recent advancements in LLM-based agents have demonstrated remarkable capabilities in handling complex, knowledge-intensive tasks by integrat…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2508.07976v4.md` · `raw/arxiv/2508.07976v4.fulltext.md`
