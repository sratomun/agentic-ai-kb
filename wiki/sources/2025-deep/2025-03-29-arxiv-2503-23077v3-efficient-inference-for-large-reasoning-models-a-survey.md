---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Efficient Inference for Large Reasoning Models: A Survey"
authors: Yue Liu, Jiaying Wu, Yufei He, Ruihan Gong et al.
url: https://arxiv.org/abs/2503.23077v3
date: 2025-03-29
citationCount: 63
influentialCitationCount: 2
velocity: 4.26
ingested: 2026-06-22
tags: [agent-security, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Efficient Inference for Large Reasoning Models: A Survey

**arXiv [2503.23077v3](https://arxiv.org/abs/2503.23077v3)** · 2025-03-29 · **63 citations** (2 influential · 4.26/mo) · Yue Liu, Jiaying Wu, Yufei He, Ruihan Gong et al.

## Abstract
Large Reasoning Models (LRMs) significantly improve the reasoning ability of Large Language Models (LLMs) by learning to reason, exhibiting promising performance in solving complex tasks. However, their deliberative reasoning process leads to inefficiencies in token usage, memory consumption, and inference time. Thus, this survey provides a review of efficient inference methods designed specifically for LRMs, focusing on mitigating token inefficiency while preserving the reasoning quality. The overview structure of this paper is shown in Figure~\ref{fig:paper_structure}. First, we introduce a taxonomy to group the recent methods into two main categories: (a) explicit compact Chain-of-Thought (CoT), which reduces tokens while keeping the explicit reasoning structure, and (b) implicit latent CoT, which encodes reasoning steps within hidden representations instead of explicit tokens. Meanwhile, we discuss their strengths and weaknesses. Then, we conduct empirical analyses on existing methods from reasoning scenarios, object functions, and performance \& efficiency aspects. Besides, we present open challenges in this field, including human-centric controllable reasoning, trade-off between interpretability and efficiency of reasoning, ensuring the safety of efficient reasoning, and broader applications of efficient reasoning. In addition, we highlight key insights for enhancing LRMs' inference efficiency via techniques such as model merging, new architectures, and agent routers. We hope this work serves as a valuable guide, helping researchers overcome challenges in this vibrant field. A collection of efficient reasoning methods for LRMs (papers and codes) is provided at this link: https://github.com/yueliu1999/Awesome-Efficient-Inference-for-LRMs.

## From the paper (full-text excerpts)
**Method / approach.** methods designed specifically for LRMs, focusing on mitigating token inefficiency while preserving the reasoning quality. The overview structure of this paper is shown in Figure 1. First, we introduce a taxonomy to group the recent methods into two main categories: (a) explicit compact Chain-ofThought (CoT), which reduces tokens while keeping the explicit reasoning structure, and (b) implicit latent CoT, which encodes reasoning steps within hidden representations instead of explicit tokens. Meanwhile, we discuss their strengths and weaknesses. Then, we conduct empirical analyses on existing methods from reasoning scenarios, object functions, and performance & efficiency aspects. Besides, we present open challenges in this field, including human-centric controllable reasoning, trade-off between interpretability and efficiency of reasoning, ensuring the safety of efficient reasoning, and broader applications of efficient reasoning. In addition, we highlight key insights for enhancing LR…

**Results.** evaluation [85] have highlighted inherent biases in automatic preference scoring, which may also affect the reliability of CoT-length optimization objectives. Figure 6. Flowchart of Reward-Based Incentivization. Each column represents one distinct kind of approach for incentivizing the token efficiency, highlighting the key steps of each method. The methods for Reward-Based Incentivization are illustrated in Figure 6. The flowchart highlights how different strategies, such as length-based rewards, harmonizing penalties, and reinforcement learning (RL) techniques, contribute to improving token efficiency in reasoning. Several works introduce length-based or harmonizing reward mechanisms: Kimi k1.5 [7] integrates lengthbased rewards to discourage verbose reasoning. O1-Pruner [47] detects ”length disharmony” and applies harmonizing penalties that promote brevity without sacrificing solution quality. TLDR [31] combines temperature scaling…

**Conclusion.** conclusion. This human-like reasoning process of LRMs can also be examined through a cognitive framework, as discussed in [13], which provides insights into the underlying mechanisms shaping model reasoning behaviors. The o1 series [4] from OpenAI, released in late 2024, marked a significant breakthrough in AI reasoning capabilities, which integrates reinforcement learning and ”Chain of-Thought” prompting [14] techniques. Following this, OpenAI released o3 [5], an upgraded version of o1, allowing it to achieve PhD-level performance in mathematics, science, and programming. Notable DeepSeek’s R1 [6] stands out for being fully open-sourced, with transparent and detailed thinking process tokens, which sets it apart from other proprietary LRMs…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.23077v3.md` · `raw/arxiv/2503.23077v3.fulltext.md`
