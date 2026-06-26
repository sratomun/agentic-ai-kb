---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ReTool: Reinforcement Learning for Strategic Tool Use in LLMs"
authors: Jiazhan Feng, Shijue Huang, Xingwei Qu, Ge Zhang et al.
url: https://arxiv.org/abs/2504.11536v2
date: 2025-04-15
citationCount: 309
influentialCitationCount: 55
velocity: 21.72
ingested: 2026-06-22
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, 2025, cited]
---

# ReTool: Reinforcement Learning for Strategic Tool Use in LLMs

**arXiv [2504.11536v2](https://arxiv.org/abs/2504.11536v2)** · 2025-04-15 · **309 citations** (55 influential · 21.72/mo) · Jiazhan Feng, Shijue Huang, Xingwei Qu, Ge Zhang et al.

## Abstract
While reasoning models (e.g., DeepSeek R1) trained with reinforcement learning (RL), excel in textual reasoning, they struggle in scenarios requiring structured problem-solving, such as geometric reasoning, concise computation, or complex equation solving-areas where computational tools like code interpreters (CI) demonstrate distinct advantages. To bridge this gap, we propose ReTool, which enhances long-form reasoning with tool-integrated learning, including two key features: (1) dynamic interleaving of real-time code execution within natural language reasoning processes, and (2) an automated RL paradigm that allows policy rollouts with multi-turn real-time code execution and teaches the model in learning when and how to invoke tools based on outcome feedback. ReTool employs a systematic training framework, beginning with synthetic cold-start data generation to produce code-augmented long-form reasoning traces for fine-tuning base models. Subsequent RL training leverages task outcomes as rewards to iteratively refine the model's tool use strategy, enabling autonomous discovery of optimal tool invocation patterns without human priors. Experiments on the challenging MATH Olympiad benchmark AIME demonstrate ReTool's superiority: Our 32B model achieves 67% accuracy with 400 training steps, outperforming text-based RL baseline (40% accuracy, 1080 steps) in efficiency and performance. Remarkably, ReTool-32B attains 72.5% accuracy in extended settings, surpassing OpenAI's o1-preview by 27.9%. Further analysis reveals emergent behaviors such as code self-correction, signaling an ''aha moment'' in which the model autonomously masters adaptive tool use. These findings highlight the promise of outcome-driven tool integration for advancing complex mathematical reasoning and offer new insights into hybrid neuro-symbolic systems.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Methodology 2.1 Overview 2.2 Cold-start for Tool-Integrated Reasoning Foundation 2.3 ReTool: Reinforcement Learning for Strategic Tool Use 2.3.1 Training Algorithm 2.3.2 Training Details 3 Experiment 3.1 Evaluation Setup 3.2 Main Results 3.3 Cognitive Analysis 4 Background and Related Work 4.1 LLM Reasoning 4.2 Tool Integrated Reasoning 5 Conclusion 6 Appendix ]ByteDance Seed \contribution [*]Co-first authors \contribution [†]Corresponding author ReTool: Reinforcement Learning for Strategic Tool Use in LLMs Jiazhan Feng Shijue Huang Xingwei Qu Ge Zhang Yujia Qin Baoquan Zhong Chengquan Jiang Jinxin Chi Wanjun Zhong [ (April 15, 2025) Abstract While reasoning models (e.g., DeepSeek R1) trained with reinforcement learning (RL), excel in textual reasoning, they struggle in scenarios requiring structured problem-solving, such as geometric reasoning, concise computation, or complex equation solving—areas where computational tools like code interpreters (CI) demonstrate distinct advantages. T…

**Method / approach.** Methodology 2.1 Overview 2.2 Cold-start for Tool-Integrated Reasoning Foundation 2.3 ReTool: Reinforcement Learning for Strategic Tool Use 2.3.1 Training Algorithm 2.3.2 Training Details 3 Experiment 3.1 Evaluation Setup 3.2 Main Results 3.3 Cognitive Analysis 4 Background and Related Work 4.1 LLM Reasoning 4.2 Tool Integrated Reasoning 5 Conclusion 6 Appendix ]ByteDance Seed \contribution [*]Co-first authors \contribution [†]Corresponding author ReTool: Reinforcement Learning for Strategic Tool Use in LLMs Jiazhan Feng Shijue Huang Xingwei Qu Ge Zhang Yujia Qin Baoquan Zhong Chengquan Jiang Jinxin Chi Wanjun Zhong [ (April 15, 2025) Abstract While reasoning models (e.g., DeepSeek R1) trained with reinforcement learning (RL), excel in textual reasoning, they struggle in scenarios requiring structured problem-solving, such as geometric reasoning, concise computation, or complex equation solving—areas where…

**Results.** Experiment 3.1 Evaluation Setup 3.2 Main Results 3.3 Cognitive Analysis 4 Background and Related Work 4.1 LLM Reasoning 4.2 Tool Integrated Reasoning 5 Conclusion 6 Appendix ]ByteDance Seed \contribution [*]Co-first authors \contribution [†]Corresponding author ReTool: Reinforcement Learning for Strategic Tool Use in LLMs Jiazhan Feng Shijue Huang Xingwei Qu Ge Zhang Yujia Qin Baoquan Zhong Chengquan Jiang Jinxin Chi Wanjun Zhong [ (April 15, 2025) Abstract While reasoning models (e.g., DeepSeek R1) trained with reinforcement learning (RL), excel in textual reasoning, they struggle in scenarios requiring structured problem-solving, such as geometric reasoning, concise computation, or complex equation solving—areas where computational tools like code interpreters (CI) demonstrate distinct advantages. To bridge this gap, we propose ReTool , which enhances long-form reasoning wit…

**Conclusion.** Conclusion 6 Appendix ]ByteDance Seed \contribution [*]Co-first authors \contribution [†]Corresponding author ReTool: Reinforcement Learning for Strategic Tool Use in LLMs Jiazhan Feng Shijue Huang Xingwei Qu Ge Zhang Yujia Qin Baoquan Zhong Chengquan Jiang Jinxin Chi Wanjun Zhong [ (April 15, 2025) Abstract While reasoning models (e.g., DeepSeek R1) trained with reinforcement learning (RL), excel in textual reasoning, they struggle in scenarios requiring structured problem-solving, such as geometric reasoning, concise computation, or complex equation solving—areas where computational tools like code interpreters (CI) demonstrate distinct advantages. To bridge this gap, we propose ReTool , which enha…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[deepseek]] · [[retool]]
- **Raw:** `raw/arxiv/2504.11536v2.md` · `raw/arxiv/2504.11536v2.fulltext.md`
