---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks"
authors: Yifei Zhou, Song Jiang, Yuandong Tian, Jason Weston et al.
url: https://arxiv.org/abs/2503.15478v1
date: 2025-03-19
citationCount: 80
influentialCitationCount: 5
velocity: 5.29
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks

**arXiv [2503.15478v1](https://arxiv.org/abs/2503.15478v1)** · 2025-03-19 · **80 citations** (5 influential · 5.29/mo) · Yifei Zhou, Song Jiang, Yuandong Tian, Jason Weston et al.

## Abstract
Large language model (LLM) agents need to perform multi-turn interactions in real-world tasks. However, existing multi-turn RL algorithms for optimizing LLM agents fail to perform effective credit assignment over multiple turns while leveraging the generalization capabilities of LLMs and it remains unclear how to develop such algorithms. To study this, we first introduce a new benchmark, ColBench, where an LLM agent interacts with a human collaborator over multiple turns to solve realistic tasks in backend programming and frontend design. Building on this benchmark, we propose a novel RL algorithm, SWEET-RL (RL with Step-WisE Evaluation from Training-time information), that uses a carefully designed optimization objective to train a critic model with access to additional training-time information. The critic provides step-level rewards for improving the policy model. Our experiments demonstrate that SWEET-RL achieves a 6% absolute improvement in success and win rates on ColBench compared to other state-of-the-art multi-turn RL algorithms, enabling Llama-3.1-8B to match or exceed the performance of GPT4-o in realistic collaborative content creation.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Collaborative Agent Benchmark (ColBench) 3.1 Design Principles 3.2 Backend Programming Collaborations 3.3 Frontend Design Collaborations 4 SWEET-RL: RL with S tep- W is E E valuation from T raining-Time Information 4.1 Problem Setup 4.2 Learning turn-wise advantage functions 4.3 Optimizing the agent by turn-wise advantage 5 Experiments 5.1 Experimental Setup 5.2 Comparisons on ColBench 5.3 Comparing other algorithms with SWEET-RL 5.4 Analysis 6 Conclusion A Hyperparameters B Theoretical Justifications C Prompts D Qualitative Comparisons of Different Credit Assignment Methods E Full Qualitative Examples 1]FAIR at Meta 2]UC Berkeley \contribution [†]Work done at Meta \contribution [*]Equal advising SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks Yifei Zhou Song Jiang Yuandong Tian Jason Weston Sergey Levine Sainbayar Sukhbaatar Xian Li [ [ yifei_zhou@berkeley (March 19, 2025) Abstract Large language model (LLM) agents need to perform multi…

**Method / approach.** Methods E Full Qualitative Examples 1]FAIR at Meta 2]UC Berkeley \contribution [†]Work done at Meta \contribution [*]Equal advising SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks Yifei Zhou Song Jiang Yuandong Tian Jason Weston Sergey Levine Sainbayar Sukhbaatar Xian Li [ [ yifei_zhou@berkeley (March 19, 2025) Abstract Large language model (LLM) agents need to perform multi-turn interactions in real-world tasks. However, existing multi-turn RL algorithms for optimizing LLM agents fail to perform effective credit assignment over multiple turns while leveraging the generalization capabilities of LLMs and it remains unclear how to develop such algorithms. To study this, we first introduce a new benchmark, ColBench, where an LLM agent interacts with a human collaborator over multiple turns to solve realistic tasks in backend programming and frontend design. Building on this benchmark, we propose a novel RL algorithm, S…

**Results.** Experiments 5.1 Experimental Setup 5.2 Comparisons on ColBench 5.3 Comparing other algorithms with SWEET-RL 5.4 Analysis 6 Conclusion A Hyperparameters B Theoretical Justifications C Prompts D Qualitative Comparisons of Different Credit Assignment Methods E Full Qualitative Examples 1]FAIR at Meta 2]UC Berkeley \contribution [†]Work done at Meta \contribution [*]Equal advising SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks Yifei Zhou Song Jiang Yuandong Tian Jason Weston Sergey Levine Sainbayar Sukhbaatar Xian Li [ [ yifei_zhou@berkeley (March 19, 2025) Abstract Large language model (LLM) agents need to perform multi-turn interactions in real-world tasks. However, existing multi-turn RL algorithms for optimizing LLM agents fail to perform effective credit assignment over multiple turns while leveraging the generalization capabilities of LLMs and…

**Conclusion.** Conclusion A Hyperparameters B Theoretical Justifications C Prompts D Qualitative Comparisons of Different Credit Assignment Methods E Full Qualitative Examples 1]FAIR at Meta 2]UC Berkeley \contribution [†]Work done at Meta \contribution [*]Equal advising SWEET-RL: Training Multi-Turn LLM Agents on Collaborative Reasoning Tasks Yifei Zhou Song Jiang Yuandong Tian Jason Weston Sergey Levine Sainbayar Sukhbaatar Xian Li [ [ yifei_zhou@berkeley (March 19, 2025) Abstract Large language model (LLM) agents need to perform multi-turn interactions in real-world tasks. However, existing multi-turn RL algorithms for optimizing LLM agents fail to perform effective credit assignment over multiple tur…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.15478v1.md` · `raw/arxiv/2503.15478v1.fulltext.md`
