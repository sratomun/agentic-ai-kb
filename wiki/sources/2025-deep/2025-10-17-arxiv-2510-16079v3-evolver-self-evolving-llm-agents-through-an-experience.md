---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle"
authors: Rong Wu, Xiaoman Wang, Jianbiao Mei, Pinlong Cai et al.
url: https://arxiv.org/abs/2510.16079v3
date: 2025-10-17
citationCount: 77
influentialCitationCount: 7
velocity: 9.45
ingested: 2026-06-22
tags: [coding-agents, self-evolving-agents, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# EvolveR: Self-Evolving LLM Agents through an Experience-Driven Lifecycle

**arXiv [2510.16079v3](https://arxiv.org/abs/2510.16079v3)** · 2025-10-17 · **77 citations** (7 influential · 9.45/mo) · Rong Wu, Xiaoman Wang, Jianbiao Mei, Pinlong Cai et al.

## Abstract
Current Large Language Model (LLM) agents show strong performance in tool use, but lack the crucial capability to systematically learn from their own experiences. While existing frameworks mainly focus on mitigating external knowledge gaps, they fail to address a more fundamental limitation: the inability to iteratively refine problem-solving strategies. In this work, we introduce EvolveR, a framework designed to enable agent to self-improve through a complete, closed-loop experience lifecycle. This lifecycle comprises two key stages: (1) Offline Self-Distillation, where the agent's interaction trajectories are synthesized into a structured repository of abstract, reusable strategic principles; (2) Online Interaction, where the agent interacts with tasks and actively retrieves distilled principles to guide its decision-making, accumulating a diverse set of behavioral trajectories. This loop employs a policy reinforcement mechanism to iteratively update the agent based on its performance. We demonstrate the effectiveness of EvolveR on complex multi-hop question-answering benchmarks, where it achieves superior performance over strong agentic baselines. Our work presents a comprehensive blueprint for agents that learn not only from external data but also from the consequences of their own actions, paving the way for more autonomous and continuously improving systems. Code is available at https://github.com/Edaizi/EvolveR.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Continual Learning and Self-Evolving Agents 2.2 LLM Agents and Reinforcement Learning 3 Method 3.1 Preliminaries: Formalizing Agent Interaction 3.2 The EvolveR Lifecycle: From Interactions to Principles 3.2.1 Offline Experience Self-Distillation Principle from Self-Distillation. Deduplication and Integration. Quality Control via Dynamic Scoring. 3.2.2 Online Interaction Experience as a Strategic Principle. Generating High-Quality Trajectories for Future Distillation. 3.3 Policy Evolution: Closing the Loop with Reinforcement Learning Reward Function. Policy Optimization. 4 Experiments 4.1 Experimental Implementation Details 4.1.1 Tasks and Datasets 4.1.2 Baseline Methods 4.1.3 Evaluation Metrics 4.1.4 Implementation Details 4.2 Main Results 5 Further Analysis 5.1 Analysis of Model Scales Generalizability 5.2 Ablation Studies: Dissecting the EvolveR Framework 5.2.1 Validating the Self-Distillation Mechanism 5.2.2 The Role of Experience Retrieval 5.2.3 Component-Level…

**Method / approach.** Method 3.1 Preliminaries: Formalizing Agent Interaction 3.2 The EvolveR Lifecycle: From Interactions to Principles 3.2.1 Offline Experience Self-Distillation Principle from Self-Distillation. Deduplication and Integration. Quality Control via Dynamic Scoring. 3.2.2 Online Interaction Experience as a Strategic Principle. Generating High-Quality Trajectories for Future Distillation. 3.3 Policy Evolution: Closing the Loop with Reinforcement Learning Reward Function. Policy Optimization. 4 Experiments 4.1 Experimental Implementation Details 4.1.1 Tasks and Datasets 4.1.2 Baseline Methods 4.1.3 Evaluation Metrics 4.1.4 Implementation Details 4.2 Main Results 5 Further Analysis 5.1 Analysis of Model Scales Generalizability 5.2 Ablation Studies: Dissecting the EvolveR Framework 5.2.1 Validating the Self-Distillation Mechanism 5.2.2 The Role of Experience Retrieval 5.2.3 Component-Level Attribution and Memory Configura…

**Results.** Experiments 4.1 Experimental Implementation Details 4.1.1 Tasks and Datasets 4.1.2 Baseline Methods 4.1.3 Evaluation Metrics 4.1.4 Implementation Details 4.2 Main Results 5 Further Analysis 5.1 Analysis of Model Scales Generalizability 5.2 Ablation Studies: Dissecting the EvolveR Framework 5.2.1 Validating the Self-Distillation Mechanism 5.2.2 The Role of Experience Retrieval 5.2.3 Component-Level Attribution and Memory Configuration 5.3 Analysis of Principle Quality and Scalability 6 Conclusion References A Appendix A.1 Experimental Implementation Details General Setup. Cold-start Stage. Online Interaction Phase. Offline Distill Phase. Reward Function Details. Policy Optimization. Computational Cost Analysis. SFT-only Baseline Details. A.2 Additional Experimental Analysis A.2.1 Necessity of the RL (GRPO) Stage A.2.2 Hyperparameter Sensitivity Analysis A.2.…

**Conclusion.** Conclusion References A Appendix A.1 Experimental Implementation Details General Setup. Cold-start Stage. Online Interaction Phase. Offline Distill Phase. Reward Function Details. Policy Optimization. Computational Cost Analysis. SFT-only Baseline Details. A.2 Additional Experimental Analysis A.2.1 Necessity of the RL (GRPO) Stage A.2.2 Hyperparameter Sensitivity Analysis A.2.3 Longitudinal Analysis of Learning Dynamics Evolution of Action Frequencies. Intrinsic Improvement in Principle Distillation. A.3 Exploring the Influence of Experience Internalization A.4 Prompt Details A.4.1 Cold Start Prompt A.4.2 System Prompt A.4.3 Distill Principle Prompt A.4.4 Judge Same Principle Pr…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[self-evolving-agents|Self-evolving agents]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.16079v3.md` · `raw/arxiv/2510.16079v3.fulltext.md`
