---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning"
authors: Sikuan Yan, Xiufeng Yang, Zuchao Huang, Ercong Nie et al.
url: https://arxiv.org/abs/2508.19828v5
date: 2025-08-27
citationCount: 127
influentialCitationCount: 18
velocity: 12.93
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning

**arXiv [2508.19828v5](https://arxiv.org/abs/2508.19828v5)** · 2025-08-27 · **127 citations** (18 influential · 12.93/mo) · Sikuan Yan, Xiufeng Yang, Zuchao Huang, Ercong Nie et al.

## Abstract
Large Language Models (LLMs) have demonstrated impressive capabilities across a wide range of NLP tasks, but they remain fundamentally stateless, constrained by limited context windows that hinder long-horizon reasoning. Recent efforts to address this limitation often augment LLMs with an external memory bank, yet most existing pipelines are static and heuristic-driven, lacking a learned mechanism for deciding what to store, update, or retrieve. We present Memory-R1, a reinforcement learning (RL) framework that equips LLMs with the ability to actively manage and utilize external memory through two specialized agents: a Memory Manager that learns structured operations, including ADD, UPDATE, DELETE, and NOOP; and an Answer Agent that pre-selects and reasons over relevant entries. Both agents are fine-tuned with outcome-driven RL (PPO and GRPO), enabling adaptive memory management with minimal supervision. With only 152 training QA pairs, Memory-R1 outperforms strong baselines and generalizes across diverse question types, three benchmarks (LoCoMo, MSC, LongMemEval), and multiple model scales (3B-14B).

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Memory Augmented LLM-based Agents 2.2 LLM and Reinforcement Learning 3 Method 3.1 RL Fine-tuning for Memory Manager Task Formulation PPO for Memory Manager GRPO for Memory Manager Reward Design for Memory Manager 3.2 RL Fine-Tuning for Answer Agent Task Formulation PPO for Answer Agent GRPO for Answer Agent Reward Design for Answer Agent 4 Experiments 4.1 Experimental Setup Dataset and Model Evaluation Metrics Baselines 4.2 Main Results 4.3 Generalization and Scalability 4.4 Ablation Studies Effect of Memory Manager Effect of Answer Agent Effect of Memory Distillation RL-Fine-Tuned Answer Agent Gains More with Stronger Memory Manager Comparison of RL Policies Reward Design Analysis Comparison of Learned Memory Distillation and Reranking 5 Conclusion A Case Study of Behavior of Agents before and after Fine-tuning A.1 From In-context Memory Manager to RL fine-tuned Memory Manager A.2 From Vanilla LLM to Memory‑Distilled RL Answer Agent B Dataset Details B.1…

**Method / approach.** Method 3.1 RL Fine-tuning for Memory Manager Task Formulation PPO for Memory Manager GRPO for Memory Manager Reward Design for Memory Manager 3.2 RL Fine-Tuning for Answer Agent Task Formulation PPO for Answer Agent GRPO for Answer Agent Reward Design for Answer Agent 4 Experiments 4.1 Experimental Setup Dataset and Model Evaluation Metrics Baselines 4.2 Main Results 4.3 Generalization and Scalability 4.4 Ablation Studies Effect of Memory Manager Effect of Answer Agent Effect of Memory Distillation RL-Fine-Tuned Answer Agent Gains More with Stronger Memory Manager Comparison of RL Policies Reward Design Analysis Comparison of Learned Memory Distillation and Reranking 5 Conclusion A Case Study of Behavior of Agents before and after Fine-tuning A.1 From In-context Memory Manager to RL fine-tuned Memory Manager A.2 From Vanilla LLM to Memory‑Distilled RL Answer Agent B Dataset Details B.1 Test Data B.2…

**Results.** Experiments 4.1 Experimental Setup Dataset and Model Evaluation Metrics Baselines 4.2 Main Results 4.3 Generalization and Scalability 4.4 Ablation Studies Effect of Memory Manager Effect of Answer Agent Effect of Memory Distillation RL-Fine-Tuned Answer Agent Gains More with Stronger Memory Manager Comparison of RL Policies Reward Design Analysis Comparison of Learned Memory Distillation and Reranking 5 Conclusion A Case Study of Behavior of Agents before and after Fine-tuning A.1 From In-context Memory Manager to RL fine-tuned Memory Manager A.2 From Vanilla LLM to Memory‑Distilled RL Answer Agent B Dataset Details B.1 Test Data B.2 Training Data C Prompts C.1 Memory Manager Prompt C.2 Answer Agent Prompt C.3 LLM-as-a-Judge (J) Prompt D Implementation Details E Alogirthm F Extended Results and Type-Level Analysis G Latency Analysis Overall Trends Memo…

**Conclusion.** Conclusion A Case Study of Behavior of Agents before and after Fine-tuning A.1 From In-context Memory Manager to RL fine-tuned Memory Manager A.2 From Vanilla LLM to Memory‑Distilled RL Answer Agent B Dataset Details B.1 Test Data B.2 Training Data C Prompts C.1 Memory Manager Prompt C.2 Answer Agent Prompt C.3 LLM-as-a-Judge (J) Prompt D Implementation Details E Alogirthm F Extended Results and Type-Level Analysis G Latency Analysis Overall Trends Memory Manager Latency Memory Search Latency Answer Agent Latency Accuracy-Latency Relationship Memory-R1: Enhancing Large Language Model Agents to Manage and Utilize Memories via Reinforcement Learning Sikuan Yan *1,2 , Xiufeng Yang *3…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]] · [[ppo]]
- **Raw:** `raw/arxiv/2508.19828v5.md` · `raw/arxiv/2508.19828v5.fulltext.md`
