---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent"
authors: Hongli Yu, Tinghong Chen, Jiangtao Feng, Jiangjie Chen et al.
url: https://arxiv.org/abs/2507.02259v1
date: 2025-07-03
citationCount: 166
influentialCitationCount: 17
velocity: 14.27
ingested: 2026-06-22
tags: [agent-memory, agentic-ai, arxiv, 2025, cited]
---

# MemAgent: Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent

**arXiv [2507.02259v1](https://arxiv.org/abs/2507.02259v1)** · 2025-07-03 · **166 citations** (17 influential · 14.27/mo) · Hongli Yu, Tinghong Chen, Jiangtao Feng, Jiangjie Chen et al.

## Abstract
Despite improvements by length extrapolation, efficient attention and memory modules, handling infinitely long documents with linear complexity without performance degradation during extrapolation remains the ultimate challenge in long-text processing. We directly optimize for long-text tasks in an end-to-end fashion and introduce a novel agent workflow, MemAgent, which reads text in segments and updates the memory using an overwrite strategy. We extend the DAPO algorithm to facilitate training via independent-context multi-conversation generation. MemAgent has demonstrated superb long-context capabilities, being able to extrapolate from an 8K context trained on 32K text to a 3.5M QA task with performance loss < 5% and achieves 95%+ in 512K RULER test.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 The Proposed MemAgent 3.1 The MemAgent Workflow: RL-shaped Memory for Unbounded Contexts 3.2 Training MemAgent with Multi-conv RL 3.3 Reward Modeling 3.4 Rethinking MemAgent from Autoregressive Modeling Perspectives 4 Experiments 4.1 Datasets 4.2 Experimental Setup 4.3 Main Results 4.4 Ablation Study 4.5 Case Study 5 Conclusion 6 Computation Complexity 7 Complete Out-Of-Domain Task Results 7.1 Needle-in-a-Haystack (NIAH) 7.2 Variable Tracking (VT) and Frequent Words Extraction (FWE) 1]ByteDance Seed 2 Institute for AI Industry Research (AIR), Tsinghua University 3 SIA-Lab of Tsinghua AIR and ByteDance Seed MemAgent : Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent Hongli Yu Tinghong Chen Jiangtao Feng Jiangjie Chen Weinan Dai Qiying Yu Ya-Qin Zhang Wei-Ying Ma Jingjing Liu Mingxuan Wang Hao Zhou [ zhouhao@air.tsinghua.edu.cn wangmingxuan.89@bytedance.com (July 2, 2025) Abstract Despite improvements by length extrapolation, efficient attention…

**Method / approach.** methods by shifting the positional embeddings in order to extend the context window of the model [ 11 , 12 , 13 , 14 , 15 ] , plus continued pre-training [ 16 , 17 , 18 ] . Despite promising potential, these methods often suffer from performance degradation and slow processing speed due to O ⁢ ( n 2 ) 𝑂 superscript 𝑛 2 O(n^{2}) italic_O ( italic_n start_POSTSUPERSCRIPT 2 end_POSTSUPERSCRIPT ) computational complexity when applied to extremely long text. The second school of methods leverages sparse attention [ 19 , 20 , 21 ] and linear attention mechanisms [ 22 , 23 ] to reduce the complexity of attention for more efficient processing of longer sequences. However, this typically requires training from scratch, with inherent adversities such as linear attention facing difficulties in parallel training or sparse attention depending on human-defined patterns. The last line of inquiry investigates context compression [ 24 , 25 , 26 , 27 ] , which aims to condense information in token…

**Results.** Experiments 4.1 Datasets 4.2 Experimental Setup 4.3 Main Results 4.4 Ablation Study 4.5 Case Study 5 Conclusion 6 Computation Complexity 7 Complete Out-Of-Domain Task Results 7.1 Needle-in-a-Haystack (NIAH) 7.2 Variable Tracking (VT) and Frequent Words Extraction (FWE) 1]ByteDance Seed 2 Institute for AI Industry Research (AIR), Tsinghua University 3 SIA-Lab of Tsinghua AIR and ByteDance Seed MemAgent : Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent Hongli Yu Tinghong Chen Jiangtao Feng Jiangjie Chen Weinan Dai Qiying Yu Ya-Qin Zhang Wei-Ying Ma Jingjing Liu Mingxuan Wang Hao Zhou [ zhouhao@air.tsinghua.edu.cn wangmingxuan.89@bytedance.com (July 2, 2025) Abstract Despite improvements by length extrapolation, efficient attention and memory modules, handling infinitely long documents with linear complexity without performance degradation during…

**Conclusion.** Conclusion 6 Computation Complexity 7 Complete Out-Of-Domain Task Results 7.1 Needle-in-a-Haystack (NIAH) 7.2 Variable Tracking (VT) and Frequent Words Extraction (FWE) 1]ByteDance Seed 2 Institute for AI Industry Research (AIR), Tsinghua University 3 SIA-Lab of Tsinghua AIR and ByteDance Seed MemAgent : Reshaping Long-Context LLM with Multi-Conv RL-based Memory Agent Hongli Yu Tinghong Chen Jiangtao Feng Jiangjie Chen Weinan Dai Qiying Yu Ya-Qin Zhang Wei-Ying Ma Jingjing Liu Mingxuan Wang Hao Zhou [ zhouhao@air.tsinghua.edu.cn wangmingxuan.89@bytedance.com (July 2, 2025) Abstract Despite improvements by length extrapolation, efficient attention and memory modules, handling infi…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2507.02259v1.md` · `raw/arxiv/2507.02259v1.fulltext.md`
