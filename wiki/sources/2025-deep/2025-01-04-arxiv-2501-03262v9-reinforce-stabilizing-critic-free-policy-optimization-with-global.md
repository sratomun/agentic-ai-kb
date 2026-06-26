---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global Advantage Normalization"
authors: Jian Hu, Jason Klein Liu, Haotian Xu, Wei Shen
url: https://arxiv.org/abs/2501.03262v9
date: 2025-01-04
citationCount: 68
influentialCitationCount: 12
velocity: 3.88
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global Advantage Normalization

**arXiv [2501.03262v9](https://arxiv.org/abs/2501.03262v9)** · 2025-01-04 · **68 citations** (12 influential · 3.88/mo) · Jian Hu, Jason Klein Liu, Haotian Xu, Wei Shen

## Abstract
Reinforcement Learning from Human Feedback~(RLHF) plays a crucial role in aligning Large Language Models~(LLMs). The dominant algorithm, Proximal Policy Optimization~(PPO), employs a critic network to estimate advantages, which introduces significant computational and memory overhead. To address this, a family of critic-free algorithms (e.g., GRPO, RLOO) has emerged. However, these methods typically rely on \textit{prompt-level (local)} advantage normalization, which suffers from inaccurate advantage estimation, a tendency to overfit, and, as we show, is a theoretically biased estimator. To solve these challenges, we introduce REINFORCE++, a critic-free framework centered on \textbf{Global Advantage Normalization}. By normalizing advantages across the entire global batch rather than small, prompt-specific groups, our method provides a more stable and theoretically sound, \textit{effectively unbiased} estimate (whose bias vanishes as batch size increases). We introduce two variants: REINFORCE++, a highly efficient and general algorithm ($k \ge 1$) for general-domain RLHF, and REINFORCE++ /w baseline, a robust group-sampling variant ($k > 1$) for complex reasoning tasks. Our empirical evaluation demonstrates that each variant shows superior stability and performance in its respective domain, outperforming existing methods and even PPO in complex agentic settings.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Background and Related Work 2.1 PPO and Critic-Free RLHF 2.2 The Problem with Local Normalization 3 Method 3.1 Global Normalization 3.2 Local Baseline 3.3 Relationship with PPO 3.4 Summary 4 Experiments 4.1 General RLHF Experimental Setup Experimental Results Results Analysis 4.2 Reasoning Experiments 4.2.1 Long Reasoning Task Analysis on Small-Scale Datasets Logical Reasoning (K K Puzzles) RL from Zero Setting 4.3 Multi-step Reinforcement Learning Experimental Setup Experimental Result 5 Best Practices 5.1 General Principle 5.2 Third-Party Validation LitePPO ScaleRL DLER 6 Conclusion A Proof: The GRPO Advantage Estimator is Biased A.1 Assumptions and Settings A.2 Why Use Global Batch Normalization? B Algorithm Details B.1 KL Penalty Design Theoretical Reverse KL Gradient k1 Analysis k2 Analysis k3 Analysis Conclusion B.2 Implementation Tricks Token-level Advantage Batch Construction Mini-Batch Updates Reward Normalization and Clipping C Acknowl…

**Method / approach.** Method 3.1 Global Normalization 3.2 Local Baseline 3.3 Relationship with PPO 3.4 Summary 4 Experiments 4.1 General RLHF Experimental Setup Experimental Results Results Analysis 4.2 Reasoning Experiments 4.2.1 Long Reasoning Task Analysis on Small-Scale Datasets Logical Reasoning (K K Puzzles) RL from Zero Setting 4.3 Multi-step Reinforcement Learning Experimental Setup Experimental Result 5 Best Practices 5.1 General Principle 5.2 Third-Party Validation LitePPO ScaleRL DLER 6 Conclusion A Proof: The GRPO Advantage Estimator is Biased A.1 Assumptions and Settings A.2 Why Use Global Batch Normalization? B Algorithm Details B.1 KL Penalty Design Theoretical Reverse KL Gradient k1 Analysis k2 Analysis k3 Analysis Conclusion B.2 Implementation Tricks Token-level Advantage Batch Construction Mini-Batch Updates Reward Normalization and Clipping C Acknowledgements REINFORCE++: S…

**Results.** Experiments 4.1 General RLHF Experimental Setup Experimental Results Results Analysis 4.2 Reasoning Experiments 4.2.1 Long Reasoning Task Analysis on Small-Scale Datasets Logical Reasoning (K K Puzzles) RL from Zero Setting 4.3 Multi-step Reinforcement Learning Experimental Setup Experimental Result 5 Best Practices 5.1 General Principle 5.2 Third-Party Validation LitePPO ScaleRL DLER 6 Conclusion A Proof: The GRPO Advantage Estimator is Biased A.1 Assumptions and Settings A.2 Why Use Global Batch Normalization? B Algorithm Details B.1 KL Penalty Design Theoretical Reverse KL Gradient k1 Analysis k2 Analysis k3 Analysis Conclusion B.2 Implementation Tricks Token-level Advantage Batch Construction Mini-Batch Updates Reward Normalization and Clipping C Acknowledgements REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global…

**Conclusion.** Conclusion A Proof: The GRPO Advantage Estimator is Biased A.1 Assumptions and Settings A.2 Why Use Global Batch Normalization? B Algorithm Details B.1 KL Penalty Design Theoretical Reverse KL Gradient k1 Analysis k2 Analysis k3 Analysis Conclusion B.2 Implementation Tricks Token-level Advantage Batch Construction Mini-Batch Updates Reward Normalization and Clipping C Acknowledgements REINFORCE++: Stabilizing Critic-Free Policy Optimization with Global Normalization Jian Hu janhu9527@gmail.com Jason Klein Liu jasonkleinlove@gmail.com Haotian Xu 1034351332@qq.com Wei Shen shenwei0917@126.com Corresponding author Abstract Reinforcement Learning from Human Feedback (RLHF)…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[ppo]]
- **Raw:** `raw/arxiv/2501.03262v9.md` · `raw/arxiv/2501.03262v9.fulltext.md`
