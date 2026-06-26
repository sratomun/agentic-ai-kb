---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agentic Reinforced Policy Optimization"
authors: Guanting Dong, Hangyu Mao, Kai Ma, Licheng Bao et al.
url: https://arxiv.org/abs/2507.19849v1
date: 2025-07-26
citationCount: 107
influentialCitationCount: 9
velocity: 9.84
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Agentic Reinforced Policy Optimization

**arXiv [2507.19849v1](https://arxiv.org/abs/2507.19849v1)** · 2025-07-26 · **107 citations** (9 influential · 9.84/mo) · Guanting Dong, Hangyu Mao, Kai Ma, Licheng Bao et al.

## Abstract
Large-scale reinforcement learning with verifiable rewards (RLVR) has demonstrated its effectiveness in harnessing the potential of large language models (LLMs) for single-turn reasoning tasks. In realistic reasoning scenarios, LLMs can often utilize external tools to assist in task-solving processes. However, current RL algorithms inadequately balance the models' intrinsic long-horizon reasoning capabilities and their proficiency in multi-turn tool interactions. To bridge this gap, we propose Agentic Reinforced Policy Optimization (ARPO), a novel agentic RL algorithm tailored for training multi-turn LLM-based agents. Through preliminary experiments, we observe that LLMs tend to exhibit highly uncertain behavior, characterized by an increase in the entropy distribution of generated tokens, immediately following interactions with external tools. Motivated by this observation, ARPO incorporates an entropy-based adaptive rollout mechanism, dynamically balancing global trajectory sampling and step-level sampling, thereby promoting exploration at steps with high uncertainty after tool usage. By integrating an advantage attribution estimation, ARPO enables LLMs to internalize advantage differences in stepwise tool-use interactions. Our experiments across 13 challenging benchmarks in computational reasoning, knowledge reasoning, and deep search domains demonstrate ARPO's superiority over trajectory-level RL algorithms. Remarkably, ARPO achieves improved performance using only half of the tool-use budget required by existing methods, offering a scalable solution for aligning LLM-based agents with real-time dynamic environments. Our code and datasets are released at https://github.com/dongguanting/ARPO

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminary 2.1 Agentic Reinforcement Learning 2.2 Analyzing Token Entropy in Agentic Reasoning 2.3 Agentic Tool Design 3 Agentic Reinforce Policy Optimization 3.1 Entropy-based Adaptive Rollout. 3.2 Advantage Attribution Estimation 3.3 Theoretical Foundation 4 Experiment 4.1 Datasets. 4.2 Baselines. 4.3 Training Guideline 4.4 Evaluation Metric 4.5 Main Results 4.6 Quantitative Analysis 4.7 Scaling Analysis of ARPO 5 Related Work 6 Conclusion A Datasets A.1 Mathematical Reasoning Benchmarks A.2 Knowledge-Intensive reasoning benchmarks A.3 Deep Search Benchmarks B Baselines B.1 Direct Reasoning B.2 Trajectory-level RL Algorithms B.3 LLM-based Search Agent C Implementation Details C.1 Supervised Fine-Tuning C.2 Reinforcement Learning C.3 Details of Search C.4 Scaling Experiment Setup C.5 C.3 D Theoretical Analysis and Proofs D.1 Theoretical Analysis of Soft Advantage Estimation D.2 Theoretical Proof of GPG Theorem D.2.1 Transformer-based Policy D.2.2 Derivation of the GP…

**Method / approach.** methods, offering a scalable solution for aligning LLM-based agents with real-time dynamic environments. Figure 1: Overview of tool-use token entropy exploration and ARPO algorithm performance. Left: High entropy observed in the LLM following tool usage. Right: LLM performance comparison on deep search tasks using only 1k RL samples , along with a comparison of training tool-use budgets. 1 Introduction Recently, large-scale Reinforcement Learning with Verifiable Rewards (RLVR) has demonstrated strong potential in unleashing the capabilities of frontier large language models (LLMs), showcasing impressive performance across various single-turn reasoning tasks (OpenAI, 2024 ; DeepSeek-AI et al., 2025 ; Team et al., 2025 ; Qwen et al., 2024 ; Yang et al., 2025 ; Yuan et al., 2023 ; He et al., 2025 ) . However, in open-ended reasoning scenarios (Putta et al., 2024 ; Shridhar et al., 2020 ; Qin et al., 2024 ; Mialon et al., 2024 ) , LLMs should not only cultivate long-horizon pl…

**Results.** Experiment 4.1 Datasets. 4.2 Baselines. 4.3 Training Guideline 4.4 Evaluation Metric 4.5 Main Results 4.6 Quantitative Analysis 4.7 Scaling Analysis of ARPO 5 Related Work 6 Conclusion A Datasets A.1 Mathematical Reasoning Benchmarks A.2 Knowledge-Intensive reasoning benchmarks A.3 Deep Search Benchmarks B Baselines B.1 Direct Reasoning B.2 Trajectory-level RL Algorithms B.3 LLM-based Search Agent C Implementation Details C.1 Supervised Fine-Tuning C.2 Reinforcement Learning C.3 Details of Search C.4 Scaling Experiment Setup C.5 C.3 D Theoretical Analysis and Proofs D.1 Theoretical Analysis of Soft Advantage Estimation D.2 Theoretical Proof of GPG Theorem D.2.1 Transformer-based Policy D.2.2 Derivation of the GPG Theorem E The Algorithm Workflow of ARPO F Case Study \pdfcolInitStack tcb@breakable Agentic Reinforced Policy Optimization Guanting Don…

**Conclusion.** Conclusion A Datasets A.1 Mathematical Reasoning Benchmarks A.2 Knowledge-Intensive reasoning benchmarks A.3 Deep Search Benchmarks B Baselines B.1 Direct Reasoning B.2 Trajectory-level RL Algorithms B.3 LLM-based Search Agent C Implementation Details C.1 Supervised Fine-Tuning C.2 Reinforcement Learning C.3 Details of Search C.4 Scaling Experiment Setup C.5 C.3 D Theoretical Analysis and Proofs D.1 Theoretical Analysis of Soft Advantage Estimation D.2 Theoretical Proof of GPG Theorem D.2.1 Transformer-based Policy D.2.2 Derivation of the GPG Theorem E The Algorithm Workflow of ARPO F Case Study \pdfcolInitStack tcb@breakable Agentic Reinforced Policy Optimization Guantin…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.19849v1.md` · `raw/arxiv/2507.19849v1.fulltext.md`
