---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Training-Free Group Relative Policy Optimization"
authors: Yuzheng Cai, Siqi Cai, Yuchen Shi, Zihan Xu et al.
url: https://arxiv.org/abs/2510.08191v1
date: 2025-10-09
citationCount: 36
influentialCitationCount: 8
velocity: 4.28
ingested: 2026-06-22
tags: [agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Training-Free Group Relative Policy Optimization

**arXiv [2510.08191v1](https://arxiv.org/abs/2510.08191v1)** · 2025-10-09 · **36 citations** (8 influential · 4.28/mo) · Yuzheng Cai, Siqi Cai, Yuchen Shi, Zihan Xu et al.

## Abstract
Recent advances in Large Language Model (LLM) agents have demonstrated their promising general capabilities. However, their performance in specialized real-world domains often degrades due to challenges in effectively integrating external tools and specific prompting strategies. While methods like agentic reinforcement learning have been proposed to address this, they typically rely on costly parameter updates, for example, through a process that uses Supervised Fine-Tuning (SFT) followed by a Reinforcement Learning (RL) phase with Group Relative Policy Optimization (GRPO) to alter the output distribution. However, we argue that LLMs can achieve a similar effect on the output distribution by learning experiential knowledge as a token prior, which is a far more lightweight approach that not only addresses practical data scarcity but also avoids the common issue of overfitting. To this end, we propose Training-Free Group Relative Policy Optimization (Training-Free GRPO), a cost-effective solution that enhances LLM agent performance without any parameter updates. Our method leverages the group relative semantic advantage instead of numerical ones within each group of rollouts, iteratively distilling high-quality experiential knowledge during multi-epoch learning on a minimal ground-truth data. Such knowledge serves as the learned token prior, which is seamlessly integrated during LLM API calls to guide model behavior. Experiments on mathematical reasoning and web searching tasks demonstrate that Training-Free GRPO, when applied to DeepSeek-V3.1-Terminus, significantly improves out-of-domain performance. With just a few dozen training samples, Training-Free GRPO outperforms fine-tuned small LLMs with marginal training data and cost.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Training-Free GRPO 3 Evalution 3.1 Mathematical Reasoning 3.2 Web Searching 4 Comparing RL Learning on Context Space and Parameter Space 4.1 Cross-domain Transfer Analysis 4.2 Computational Costs 5 Related Work 6 Conclusion A Case Study A.1 Experience-Guided Tool-Integrated Math Reasoning A.2 Experience-Guided Web Searching B Prompts C Examples of Learned Experiences \correspondence tristanli@tencent.com \sourcecode https://github.com/TencentCloudADP/youtu-agent/tree/training_free_GRPO Training-Free Group Relative Policy Optimization (October 9, 2025) Abstract Recent advances in Large Language Model (LLM) agents have demonstrated their promising general capabilities. However, their performance in specialized real-world domains often degrades due to challenges in effectively integrating external tools and specific prompting strategies. While methods like agentic reinforcement learning have been proposed to address this, they typically rely on costly parameter updates, for example, through a process that uses Super…

**Method / approach.** methods like agentic reinforcement learning have been proposed to address this, they typically rely on costly parameter updates, for example, through a process that uses Supervised Fine-Tuning (SFT) followed by a Reinforcement Learning (RL) phase with Group Relative Policy Optimization (GRPO) to alter the output distribution. However, we argue that LLMs can achieve a similar effect on the output distribution by learning experiential knowledge as a token prior, which is a far more lightweight approach that not only addresses practical data scarcity but also avoids the common issue of overfitting. To this end, we propose Training-Free Group Relative Policy Optimization (Training-Free GRPO), a cost-effective solution that enhances LLM agent performance without any parameter updates. Our method leverages the group relative semantic advantage instead of numerical ones within each group of rollouts, iteratively distilling high-quality experiential knowledge during multi-epoch learning on a…

**Results.** Experiments on mathematical reasoning and web searching tasks demonstrate that Training-Free GRPO, when applied to DeepSeek-V3.1-Terminus, significantly improves out-of-domain performance. With just a few dozen training samples, Training-Free GRPO outperforms fine-tuned small LLMs with marginal training data and cost. Figure 1 : Applying Training-Free GRPO on both prompting (without tools) and ReAct [ 1 ] (with tools) achieve improved Mean@32 on AIME benchmarks [ 2 ] with DeepSeek-V3.1-Terminus [ 3 ] . It consumes significantly fewer training data and lower costs on the 671B LLM than fine-tuning a 32B model [ 4 ] , serving as a cost-effective alternative to RL methods. * * footnotetext: Full author list in contributions. 1 Introduction Large Language Models (LLMs) are emerging as powerful general-purpose agents capable of interacting with complex, real-world environments. They have shown remarkable capabilities across a…

**Conclusion.** Conclusion A Case Study A.1 Experience-Guided Tool-Integrated Math Reasoning A.2 Experience-Guided Web Searching B Prompts C Examples of Learned Experiences \correspondence tristanli@tencent.com \sourcecode https://github.com/TencentCloudADP/youtu-agent/tree/training_free_GRPO Training-Free Group Relative Policy Optimization (October 9, 2025) Abstract Recent advances in Large Language Model (LLM) agents have demonstrated their promising general capabilities. However, their performance in specialized real-world domains often degrades due to challenges in effectively integrating external tools and specific prompting strategies. While methods like agentic reinforcement learning have been proposed to address this,…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[deepseek]]
- **Raw:** `raw/arxiv/2510.08191v1.md` · `raw/arxiv/2510.08191v1.fulltext.md`
