---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Tool-Star: Empowering LLM-Brained Multi-Tool Reasoner via Reinforcement Learning"
authors: Guanting Dong, Yifei Chen, Xiaoxi Li, Jiajie Jin et al.
url: https://arxiv.org/abs/2505.16410v1
date: 2025-05-22
citationCount: 50
influentialCitationCount: 6
velocity: 3.84
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# Tool-Star: Empowering LLM-Brained Multi-Tool Reasoner via Reinforcement Learning

**arXiv [2505.16410v1](https://arxiv.org/abs/2505.16410v1)** · 2025-05-22 · **50 citations** (6 influential · 3.84/mo) · Guanting Dong, Yifei Chen, Xiaoxi Li, Jiajie Jin et al.

## Abstract
Recently, large language models (LLMs) have shown remarkable reasoning capabilities via large-scale reinforcement learning (RL). However, leveraging the RL algorithm to empower effective multi-tool collaborative reasoning in LLMs remains an open challenge. In this paper, we introduce Tool-Star, an RL-based framework designed to empower LLMs to autonomously invoke multiple external tools during stepwise reasoning. Tool-Star integrates six types of tools and incorporates systematic designs in both data synthesis and training. To address the scarcity of tool-use data, we propose a general tool-integrated reasoning data synthesis pipeline, which combines tool-integrated prompting with hint-based sampling to automatically and scalably generate tool-use trajectories. A subsequent quality normalization and difficulty-aware classification process filters out low-quality samples and organizes the dataset from easy to hard. Furthermore, we propose a two-stage training framework to enhance multi-tool collaborative reasoning by: (1) cold-start fine-tuning, which guides LLMs to explore reasoning patterns via tool-invocation feedback; and (2) a multi-tool self-critic RL algorithm with hierarchical reward design, which reinforces reward understanding and promotes effective tool collaboration. Experimental analyses on over 10 challenging reasoning benchmarks highlight the effectiveness and efficiency of Tool-Star. The code is available at https://github.com/dongguanting/Tool-Star.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Tool-Integrated Reasoning. 3 Methodology 3.1 Tool-Integrated Reasoning Data Synthesis 3.1.1 Step-1: Data Collection and Sampling 3.1.2 Step-2: Tool-Use Quality Normalization. 3.1.3 Step-3: Difficulty-Aware Data Classification. 3.2 Tool-Star: A Two-stage Multi-tool Collaborative Training Framework 3.3 Multi-tool Collaborative Inference 4 Experiments 4.1 Results on Challenging Reasoning Tasks 4.2 Quantitative Analysis 5 Conclusion A Supplement Experimental Results A.1 Deep Web Exploration Result A.2 Different RL Algorithm: REINFORCE++ VS. GRPO A.3 Analysis of Tool-Call Masking B Details of Tool-Star Framework B.1 Training Algorithm of Tool-Star B.2 Details of Tool Design C Implementation Details C.1 The Statistics of Data Sources C.2 Training Details of Tool-Star Cold-Start Supervised Finetuning. Multi-Tool Self-Critic Reinforcement Learning. Self-Critic DPO Training. C.3 Details of Retrieval C.4 Baseline Details C.5 Datasets Details D Instruction Templates D.1 Instr…

**Method / approach.** Methodology 3.1 Tool-Integrated Reasoning Data Synthesis 3.1.1 Step-1: Data Collection and Sampling 3.1.2 Step-2: Tool-Use Quality Normalization. 3.1.3 Step-3: Difficulty-Aware Data Classification. 3.2 Tool-Star: A Two-stage Multi-tool Collaborative Training Framework 3.3 Multi-tool Collaborative Inference 4 Experiments 4.1 Results on Challenging Reasoning Tasks 4.2 Quantitative Analysis 5 Conclusion A Supplement Experimental Results A.1 Deep Web Exploration Result A.2 Different RL Algorithm: REINFORCE++ VS. GRPO A.3 Analysis of Tool-Call Masking B Details of Tool-Star Framework B.1 Training Algorithm of Tool-Star B.2 Details of Tool Design C Implementation Details C.1 The Statistics of Data Sources C.2 Training Details of Tool-Star Cold-Start Supervised Finetuning. Multi-Tool Self-Critic Reinforcement Learning. Self-Critic DPO Training. C.3 Details of Retrieval C.4 Baseline Details C.5 Datasets Details D In…

**Results.** Experiments 4.1 Results on Challenging Reasoning Tasks 4.2 Quantitative Analysis 5 Conclusion A Supplement Experimental Results A.1 Deep Web Exploration Result A.2 Different RL Algorithm: REINFORCE++ VS. GRPO A.3 Analysis of Tool-Call Masking B Details of Tool-Star Framework B.1 Training Algorithm of Tool-Star B.2 Details of Tool Design C Implementation Details C.1 The Statistics of Data Sources C.2 Training Details of Tool-Star Cold-Start Supervised Finetuning. Multi-Tool Self-Critic Reinforcement Learning. Self-Critic DPO Training. C.3 Details of Retrieval C.4 Baseline Details C.5 Datasets Details D Instruction Templates D.1 Instructions for Tool-Star D.2 Instructions for Code Debugger D.3 Instructions for Reasoning Chain Refiner D.4 Instructions for Standard RAG D.5 Instructions for Knowledge-Intensive Reasoning Model D.6 Instructions for Computational Reasoni…

**Conclusion.** Conclusion A Supplement Experimental Results A.1 Deep Web Exploration Result A.2 Different RL Algorithm: REINFORCE++ VS. GRPO A.3 Analysis of Tool-Call Masking B Details of Tool-Star Framework B.1 Training Algorithm of Tool-Star B.2 Details of Tool Design C Implementation Details C.1 The Statistics of Data Sources C.2 Training Details of Tool-Star Cold-Start Supervised Finetuning. Multi-Tool Self-Critic Reinforcement Learning. Self-Critic DPO Training. C.3 Details of Retrieval C.4 Baseline Details C.5 Datasets Details D Instruction Templates D.1 Instructions for Tool-Star D.2 Instructions for Code Debugger D.3 Instructions for Reasoning Chain Refiner D.4 Instructions for Standard R…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2505.16410v1.md` · `raw/arxiv/2505.16410v1.fulltext.md`
