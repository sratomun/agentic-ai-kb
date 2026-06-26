---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning"
authors: Shulin Tian, Ruiqi Wang, Hongming Guo, Penghao Wu et al.
url: https://arxiv.org/abs/2506.13654v1
date: 2025-06-16
citationCount: 51
influentialCitationCount: 6
velocity: 4.18
ingested: 2026-06-22
tags: [agentic-rl, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning

**arXiv [2506.13654v1](https://arxiv.org/abs/2506.13654v1)** · 2025-06-16 · **51 citations** (6 influential · 4.18/mo) · Shulin Tian, Ruiqi Wang, Hongming Guo, Penghao Wu et al.

## Abstract
We introduce Ego-R1, a novel framework for reasoning over ultra-long (i.e., in days and weeks) egocentric videos, which leverages a structured Chain-of-Tool-Thought (CoTT) process, orchestrated by an Ego-R1 Agent trained via reinforcement learning (RL). Inspired by human problem-solving strategies, CoTT decomposes complex reasoning into modular steps, with the RL agent invoking specific tools, one per step, to iteratively and collaboratively answer sub-questions tackling such tasks as temporal retrieval and multi-modal understanding. We design a two-stage training paradigm involving supervised finetuning (SFT) of a pretrained language model using CoTT data and RL to enable our agent to dynamically propose step-by-step tools for long-range reasoning. To facilitate training, we construct a dataset called Ego-R1 Data, which consists of Ego-CoTT-25K for SFT and Ego-QA-4.4K for RL. Furthermore, our Ego-R1 agent is evaluated on a newly curated week-long video QA benchmark, Ego-R1 Bench, which contains human-verified QA pairs from hybrid sources. Extensive results demonstrate that the dynamic, tool-augmented chain-of-thought reasoning by our Ego-R1 Agent can effectively tackle the unique challenges of understanding ultra-long egocentric videos, significantly extending the time coverage from few hours to a week.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Egocentric Long Video Reasoning via Dynamic Tool-Calling 3.1 Egocentric Long Video Reasoning Tasks 3.2 Dynamic Tool-Calling 4 Ego-R1 Data: Chain-of-Tool-Thought (CoTT) for Video Reasoning 4.1 Chain-of-Tool-Thought (CoTT) 4.2 Data Generation 5 Ego-R1 Agent: Towards Tools Integrated Video Understanding Agent 5.1 Stage 1: Supervised fine-tuning (SFT) 5.2 Stage 2: Reinforcement learning (RL) 6 Experiments 6.1 Experiment Setup Benchmarks. Comparison Methods. 6.2 Results Exocentric setting. Egocentric settings. Analysis. 6.3 Ablation Study 7 Conclusion and Outlook 8 Acknowledgment A Hierarchical RAG B Implementation Details B.1 Environment Setup B.2 Data Generation B.3 RAG Construction for Other Benchmarks C Additional Experiments C.1 Ablation Studies C.2 Qualitative Results D Future Works Social-behaviour analysis. Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning Shulin Tian 1,2∗ Ruiqi Wang 1,3∗ Hongming Guo 4 Penghao Wu 1 Yuhao Dong…

**Method / approach.** Methods. 6.2 Results Exocentric setting. Egocentric settings. Analysis. 6.3 Ablation Study 7 Conclusion and Outlook 8 Acknowledgment A Hierarchical RAG B Implementation Details B.1 Environment Setup B.2 Data Generation B.3 RAG Construction for Other Benchmarks C Additional Experiments C.1 Ablation Studies C.2 Qualitative Results D Future Works Social-behaviour analysis. Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning Shulin Tian 1,2∗ Ruiqi Wang 1,3∗ Hongming Guo 4 Penghao Wu 1 Yuhao Dong 1 Xiuying Wang 1 Jingkang Yang 1 Hao Zhang 3 Hongyuan Zhu 2 Ziwei Liu 1 1 S-Lab, Nanyang Technological University 2 A*STAR, Singapore 3 Simon Fraser University 4 Shanghai AI Lab Abstract We introduce Ego-R1 , a novel framework for reasoning over ultra-long (i.e., in days and weeks) egocentric videos, which leverages a structured Chain-of-Tool-Thought (CoTT) process, orchestrated by an Ego-R1 Ag…

**Results.** Experiments 6.1 Experiment Setup Benchmarks. Comparison Methods. 6.2 Results Exocentric setting. Egocentric settings. Analysis. 6.3 Ablation Study 7 Conclusion and Outlook 8 Acknowledgment A Hierarchical RAG B Implementation Details B.1 Environment Setup B.2 Data Generation B.3 RAG Construction for Other Benchmarks C Additional Experiments C.1 Ablation Studies C.2 Qualitative Results D Future Works Social-behaviour analysis. Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning Shulin Tian 1,2∗ Ruiqi Wang 1,3∗ Hongming Guo 4 Penghao Wu 1 Yuhao Dong 1 Xiuying Wang 1 Jingkang Yang 1 Hao Zhang 3 Hongyuan Zhu 2 Ziwei Liu 1 1 S-Lab, Nanyang Technological University 2 A*STAR, Singapore 3 Simon Fraser University 4 Shanghai AI Lab Abstract We introduce Ego-R1 , a novel framework for reasoning over ultra-long (i.e., in days and weeks)…

**Conclusion.** Conclusion and Outlook 8 Acknowledgment A Hierarchical RAG B Implementation Details B.1 Environment Setup B.2 Data Generation B.3 RAG Construction for Other Benchmarks C Additional Experiments C.1 Ablation Studies C.2 Qualitative Results D Future Works Social-behaviour analysis. Ego-R1: Chain-of-Tool-Thought for Ultra-Long Egocentric Video Reasoning Shulin Tian 1,2∗ Ruiqi Wang 1,3∗ Hongming Guo 4 Penghao Wu 1 Yuhao Dong 1 Xiuying Wang 1 Jingkang Yang 1 Hao Zhang 3 Hongyuan Zhu 2 Ziwei Liu 1 1 S-Lab, Nanyang Technological University 2 A*STAR, Singapore 3 Simon Fraser University 4 Shanghai AI Lab Abstract We introduce Ego-R1 , a novel framework for reasoning over ultra-long (…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2506.13654v1.md` · `raw/arxiv/2506.13654v1.fulltext.md`
