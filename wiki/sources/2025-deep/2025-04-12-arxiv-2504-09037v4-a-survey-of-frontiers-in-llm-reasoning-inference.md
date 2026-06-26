---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason, and Agentic Systems"
authors: Zixuan Ke, Fangkai Jiao, Yifei Ming, Xuan-Phi Nguyen et al.
url: https://arxiv.org/abs/2504.09037v4
date: 2025-04-12
citationCount: 112
influentialCitationCount: 1
velocity: 7.82
ingested: 2026-06-22
tags: [agentic-rl, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason, and Agentic Systems

**arXiv [2504.09037v4](https://arxiv.org/abs/2504.09037v4)** · 2025-04-12 · **112 citations** (1 influential · 7.82/mo) · Zixuan Ke, Fangkai Jiao, Yifei Ming, Xuan-Phi Nguyen et al.

## Abstract
Reasoning is a fundamental cognitive process that enables logical inference, problem-solving, and decision-making. With the rapid advancement of large language models (LLMs), reasoning has emerged as a key capability that distinguishes advanced AI systems from conventional models that empower chatbots. In this survey, we categorize existing methods along two orthogonal dimensions: (1) Regimes, which define the stage at which reasoning is achieved (either at inference time or through dedicated training); and (2) Architectures, which determine the components involved in the reasoning process, distinguishing between standalone LLMs and agentic compound systems that incorporate external tools, and multi-agent collaborations. Within each dimension, we analyze two key perspectives: (1) Input level, which focuses on techniques that construct high-quality prompts that the LLM condition on; and (2) Output level, which methods that refine multiple sampled candidates to enhance reasoning quality. This categorization provides a systematic understanding of the evolving landscape of LLM reasoning, highlighting emerging trends such as the shift from inference-scaling to learning-to-reason (e.g., DeepSeek-R1), and the transition to agentic workflows (e.g., OpenAI Deep Research, Manus Agent). Additionally, we cover a broad spectrum of learning algorithms, from supervised fine-tuning to reinforcement learning such as PPO and GRPO, and the training of reasoners and verifiers. We also examine key designs of agentic workflows, from established patterns like generator-evaluator and LLM debate to recent innovations. ...

## From the paper (full-text excerpts)
**Introduction.** Introduction 1.1 Reasoning Regimes Inference scaling Learning-to-reason 1.2 Reasoning System Architecture Standalone LLM and agentic systems Single-Agent and multi-agent systems 1.3 Unified Perspectives 1.4 Goal and Structure of the Survey 1.5 Comparison to Related Surveys 2 Background 2.1 Problem Formulation Reasoning step and thought Reasoning as MDP 2.2 Key Components of LLM Reasoning Systems Reasoner Verifier Refiner 2.3 System Architectures 2.3.1 Standalone LLM Systems 2.3.2 From Standalone LLM to Language Agents 2.3.3 Single-agent Systems 2.3.4 Multi-agent Systems 2.4 Reasoning Regimes 2.4.1 Inference Scaling 2.4.2 Learning to Reason 3 Improving Reasoning with Inference Scaling 3.1 Inference Scaling With Standalone LLM 3.1.1 Constructing Reasoning Provoking Prompts Instruction engineering Demonstration engineering Prompt optimization 3.1.2 Optimizing Reasoning Output with Search and Planning Generating reasoning subtasks Exploration and search 3.2 Inference Scaling With Single-age…

**Method / approach.** methods along two orthogonal dimensions: (1) Regimes , which define the stage at which reasoning is achieved (either at inference time or through dedicated training); and (2) Architectures , which determine the components involved in the reasoning process, distinguishing between standalone LLMs and agentic compound systems that incorporate external tools, and multi-agent collaborations. Within each dimension, we analyze two key perspectives: (1) Input level, which focuses on techniques that construct high-quality prompts that the LLM condition on; and (2) Output level, which methods that refine multiple sampled candidates to enhance reasoning quality. This categorization provides a systematic understanding of the evolving landscape of LLM reasoning, highlighting emerging trends such as the shift from inference-scaling to learning-to-reason (e.g., DeepSeek-R1), and the transition to agentic workflows (e.g., OpenAI Deep Research, Manus Agent). Additionally, we cover a broad spectrum of…

**Results.** evaluation as a reasoning task 6.2 Open Challenges 6.2.1 Evaluating Reasoning 6.2.2 Understanding Reasoning Empirical analysis of reasoning Formal analysis of reasoning Theoretical analysis of ICL and CoT reasoning 6.2.3 Data Challenges in Advancing Reasoning Capabilities Challenges in scaling question and outcome supervision for RL Challenges in reward modeling 7 Conclusion References License: CC BY 4.0 arXiv:2504.09037v4 [cs.AI] 17 Mar 2026 A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason, and Agentic Systems Zixuan Ke ⋆ zixuan.ke@salesforce.com Fangkai Jiao ⋄,‡ jiaofangkai@hotmail.com Yifei Ming ⋆ yifei.ming@salesforce.com Xuan-Phi Nguyen ⋆ xnguyen@salesforce.com Austin Xu ⋆ austin.xu@salesforce.com Do Xuan Long †,‡ xuanlong.do@u.nus.edu Minzhi Li † ‡ {}^{\dagger\,\ddagger} li.minzhi@u.nus.edu Chengwei Qin ♣ chengweiqin@hkust-gz.edu.cn Peifeng W…

**Conclusion.** Conclusion References License: CC BY 4.0 arXiv:2504.09037v4 [cs.AI] 17 Mar 2026 A Survey of Frontiers in LLM Reasoning: Inference Scaling, Learning to Reason, and Agentic Systems Zixuan Ke ⋆ zixuan.ke@salesforce.com Fangkai Jiao ⋄,‡ jiaofangkai@hotmail.com Yifei Ming ⋆ yifei.ming@salesforce.com Xuan-Phi Nguyen ⋆ xnguyen@salesforce.com Austin Xu ⋆ austin.xu@salesforce.com Do Xuan Long †,‡ xuanlong.do@u.nus.edu Minzhi Li † ‡ {}^{\dagger\,\ddagger} li.minzhi@u.nus.edu Chengwei Qin ♣ chengweiqin@hkust-gz.edu.cn Peifeng Wang ⋆ peifeng.wang@salesforce.com Silvio Savarese ⋆ ssavarese@salesforce.com Caiming Xiong ⋆ cxiong@salesforce.com Shafiq Joty ⋆,⋄ sjoty@salesforce.com ⋆ Salesforce AI Research…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[ppo]] · [[deepseek]]
- **Raw:** `raw/arxiv/2504.09037v4.md` · `raw/arxiv/2504.09037v4.fulltext.md`
