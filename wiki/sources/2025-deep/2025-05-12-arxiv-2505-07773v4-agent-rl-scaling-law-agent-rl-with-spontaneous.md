---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Agent RL Scaling Law: Agent RL with Spontaneous Code Execution for Mathematical Problem Solving"
authors: Xinji Mai, Haotian Xu, Zhong-Zhi Li, Xing W et al.
url: https://arxiv.org/abs/2505.07773v4
date: 2025-05-12
citationCount: 53
influentialCitationCount: 6
velocity: 3.97
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Agent RL Scaling Law: Agent RL with Spontaneous Code Execution for Mathematical Problem Solving

**arXiv [2505.07773v4](https://arxiv.org/abs/2505.07773v4)** · 2025-05-12 · **53 citations** (6 influential · 3.97/mo) · Xinji Mai, Haotian Xu, Zhong-Zhi Li, Xing W et al.

## Abstract
Large Language Models (LLMs) often struggle with mathematical reasoning tasks requiring precise, verifiable computation. While Reinforcement Learning (RL) from outcome-based rewards enhances text-based reasoning, understanding how agents autonomously learn to leverage external tools like code execution remains crucial. We investigate RL from outcome-based rewards for Tool-Integrated Reasoning, ZeroTIR, training base LLMs to spontaneously generate and execute Python code for mathematical problems without supervised tool-use examples. Our central contribution is we demonstrate that as RL training progresses, key metrics scale predictably. Specifically, we observe strong positive correlations where increased training steps lead to increases in the spontaneous code execution frequency, the average response length, and, critically, the final task accuracy. This suggests a quantifiable relationship between computational effort invested in training and the emergence of effective, tool-augmented reasoning strategies. We implement a robust framework featuring a decoupled code execution environment and validate our findings across standard RL algorithms and frameworks. Experiments show ZeroTIR significantly surpasses non-tool ZeroRL baselines on challenging math benchmarks. Our findings provide a foundational understanding of how autonomous tool use is acquired and scales within Agent RL, offering a reproducible benchmark for future studies. Code is released at \href{https://github.com/yyht/openrlhf_async_pipline}{https://github.com/yyht/openrlhf\_async\_pipline}.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Tool-Integrated Reasoning 2.2 Agent Reinforcement Learning 3 Methodology 3.1 RL for Spontaneous Code Execution 3.2 Training Stability and Efficiency Techniques 3.3 Environment Interaction Frameworks 4 Experiments 4.1 Experimental Setup 4.2 Comparative Performance Analysis 4.3 Analysis of hyperparameters 4.4 Analysis of Training Dynamics 4.5 Joint scaling of training and inference-time interactions 5 Conclusion Agent RL Scaling Law: Spontaneous Code Execution for Mathematical Problem Solving Xinji Mai 1,2† Haotian Xu 2† Zhong-Zhi Li 5 Xing W 2 Weinong Wang 2 Jian Hu 4 Yingying Zhang 3∗ Wenqiang Zhang 1∗ 1 Fudan University 2 Xiaohongshu 3 East China Normal University 4 Independent Researcher 5 University of Chinese Academy of Sciences xjmai23@m.fudan.edu.cn,{xuhaotian,wuxing,wangweinong}@xiaohongshu.com lizhongzhi2022@ia.ac.cn , janhu9527@gmail.com Abstract Large Language Models (LLMs) often struggle with mathematical reasoning tasks requiring precise, verifiable computation. While Rei…

**Method / approach.** Methodology 3.1 RL for Spontaneous Code Execution 3.2 Training Stability and Efficiency Techniques 3.3 Environment Interaction Frameworks 4 Experiments 4.1 Experimental Setup 4.2 Comparative Performance Analysis 4.3 Analysis of hyperparameters 4.4 Analysis of Training Dynamics 4.5 Joint scaling of training and inference-time interactions 5 Conclusion Agent RL Scaling Law: Spontaneous Code Execution for Mathematical Problem Solving Xinji Mai 1,2† Haotian Xu 2† Zhong-Zhi Li 5 Xing W 2 Weinong Wang 2 Jian Hu 4 Yingying Zhang 3∗ Wenqiang Zhang 1∗ 1 Fudan University 2 Xiaohongshu 3 East China Normal University 4 Independent Researcher 5 University of Chinese Academy of Sciences xjmai23@m.fudan.edu.cn,{xuhaotian,wuxing,wangweinong}@xiaohongshu.com lizhongzhi2022@ia.ac.cn , janhu9527@gmail.com Abstract Large Language Models (LLMs) often struggle with mathematical reasoning tasks requiring precise, verifiable computation. While Reinforce…

**Results.** Experiments 4.1 Experimental Setup 4.2 Comparative Performance Analysis 4.3 Analysis of hyperparameters 4.4 Analysis of Training Dynamics 4.5 Joint scaling of training and inference-time interactions 5 Conclusion Agent RL Scaling Law: Spontaneous Code Execution for Mathematical Problem Solving Xinji Mai 1,2† Haotian Xu 2† Zhong-Zhi Li 5 Xing W 2 Weinong Wang 2 Jian Hu 4 Yingying Zhang 3∗ Wenqiang Zhang 1∗ 1 Fudan University 2 Xiaohongshu 3 East China Normal University 4 Independent Researcher 5 University of Chinese Academy of Sciences xjmai23@m.fudan.edu.cn,{xuhaotian,wuxing,wangweinong}@xiaohongshu.com lizhongzhi2022@ia.ac.cn , janhu9527@gmail.com Abstract Large Language Models (LLMs) often struggle with mathematical reasoning tasks requiring precise, verifiable computation. While Reinforcement Learning (RL) from outcome-based rewards enhances text-based reasoning, understanding how agents…

**Conclusion.** Conclusion Agent RL Scaling Law: Spontaneous Code Execution for Mathematical Problem Solving Xinji Mai 1,2† Haotian Xu 2† Zhong-Zhi Li 5 Xing W 2 Weinong Wang 2 Jian Hu 4 Yingying Zhang 3∗ Wenqiang Zhang 1∗ 1 Fudan University 2 Xiaohongshu 3 East China Normal University 4 Independent Researcher 5 University of Chinese Academy of Sciences xjmai23@m.fudan.edu.cn,{xuhaotian,wuxing,wangweinong}@xiaohongshu.com lizhongzhi2022@ia.ac.cn , janhu9527@gmail.com Abstract Large Language Models (LLMs) often struggle with mathematical reasoning tasks requiring precise, verifiable computation. While Reinforcement Learning (RL) from outcome-based rewards enhances text-based reasoning, understanding how agents autonomously lear…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2505.07773v4.md` · `raw/arxiv/2505.07773v4.fulltext.md`
