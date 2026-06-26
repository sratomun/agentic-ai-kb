---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Multi-Agent Evolve: LLM Self-Improve through Co-evolution"
authors: Yixing Chen, Yiding Wang, Siqi Zhu, Haofei Yu et al.
url: https://arxiv.org/abs/2510.23595v3
date: 2025-10-27
citationCount: 37
influentialCitationCount: 7
velocity: 4.73
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Multi-Agent Evolve: LLM Self-Improve through Co-evolution

**arXiv [2510.23595v3](https://arxiv.org/abs/2510.23595v3)** · 2025-10-27 · **37 citations** (7 influential · 4.73/mo) · Yixing Chen, Yiding Wang, Siqi Zhu, Haofei Yu et al.

## Abstract
Reinforcement Learning (RL) has demonstrated significant potential in enhancing the reasoning capabilities of large language models (LLMs). However, the success of RL for LLMs heavily relies on human-curated datasets and verifiable rewards, which limit their scalability and generality. Recent Self-Play RL methods, inspired by the success of the paradigm in games and Go, aim to enhance LLM reasoning capabilities without human-annotated data. However, their methods primarily depend on a grounded environment for feedback (e.g., a Python interpreter or a game engine); extending them to general domains remains challenging. To address these challenges, we propose Multi-Agent Evolve (MAE), a framework that enables LLMs to self-evolve in solving diverse tasks, including mathematics, reasoning, and general knowledge Q&A. The core design of MAE is based on a triplet of interacting agents (Proposer, Solver, Judge) that are instantiated from a single LLM, and applies reinforcement learning to optimize their behaviors. The Proposer generates questions, the Solver attempts solutions, and the Judge evaluates both while co-evolving. Experiments on Qwen2.5-3B-Instruct demonstrate that MAE achieves an average improvement of 4.54% on multiple benchmarks. These results highlight MAE as a scalable, data-efficient method for enhancing the general reasoning abilities of LLMs with minimal reliance on human-curated supervision.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works LLM-as-a-judge Self-Play for LLM Multi-Agent for LLM 3 Preliminaries Zero-Sum Self-Play Task-Relative REINFORCE++ 4 Multi-Agent Evolve 4.1 The Proposer Reward Design. Quality Filtering 4.2 The Solver Reward Design 4.3 The Judge Judging Answers Judging Questions Format Reward 4.4 Coordination among Proposer, Solver, and Judge 5 Experiments Settings: Baselines: 5.1 Results and Findings Evolution without Reference Questions Evolution with Reference Questions 5.2 Training Stability and Training Curve Analysis 5.2.1 Training Stability 5.2.2 Training Curve Analysis Agent diversity contributes to stability Desirable difficulty offers improvement 5.3 Ablation 5.3.1 Agent Roles 5.3.2 Format Reward and Question Quality Filtering 6 Conclusion A Prompts and Training Hyperparameters A.1 Prompts for Agents A.2 Training Hyperparameters B Evaluation Prompts and Configuration B.1 Prompts for evaluating math problems B.2 Prompts for evaluating multiple c…

**Method / approach.** methods, inspired by the success of the paradigm in games and Go, aim to enhance LLM reasoning capabilities without human-annotated data. However, their methods primarily depend on a grounded environment for feedback ( e.g. , a Python interpreter or a game engine); extending them to general domains remains challenging. To address these challenges, we propose Multi-Agent Evolve (MAE) , a framework that enables LLMs to self-evolve in solving diverse tasks, including mathematics, reasoning, and general knowledge Q A. The core design of MAE is based on a triplet of interacting agents ( Proposer , Solver , Judge ) that are instantiated from a single LLM, and applies reinforcement learning to optimize their behaviors. The Proposer generates questions, the Solver attempts solutions, and the Judge evaluates both while co-evolving. Experiments on Qwen2.5-3B-Instruct demonstrate that MAE achieves an average improvement of 4.54% on multiple benchmarks. These results highlight MAE as a scalable,…

**Results.** Experiments Settings: Baselines: 5.1 Results and Findings Evolution without Reference Questions Evolution with Reference Questions 5.2 Training Stability and Training Curve Analysis 5.2.1 Training Stability 5.2.2 Training Curve Analysis Agent diversity contributes to stability Desirable difficulty offers improvement 5.3 Ablation 5.3.1 Agent Roles 5.3.2 Format Reward and Question Quality Filtering 6 Conclusion A Prompts and Training Hyperparameters A.1 Prompts for Agents A.2 Training Hyperparameters B Evaluation Prompts and Configuration B.1 Prompts for evaluating math problems B.2 Prompts for evaluating multiple choice problems B.3 Prompts for evaluating truthfulness problems B.4 Prompts for evaluating other general problems B.5 Evaluation Configuration C Generation Examples C.1 Proposer C.2 Solver C.3 Judge D Seed Data Composition Multi-Agent Evolve:…

**Conclusion.** Conclusion A Prompts and Training Hyperparameters A.1 Prompts for Agents A.2 Training Hyperparameters B Evaluation Prompts and Configuration B.1 Prompts for evaluating math problems B.2 Prompts for evaluating multiple choice problems B.3 Prompts for evaluating truthfulness problems B.4 Prompts for evaluating other general problems B.5 Evaluation Configuration C Generation Examples C.1 Proposer C.2 Solver C.3 Judge D Seed Data Composition Multi-Agent Evolve: LLM Self-Improve through Co-evolution Yixing Chen † 1 {}^{1}{{}^{\dagger}} Yiding Wang † 1 {}^{1}{{}^{\dagger}} 1 1 footnotemark: 1 Siqi Zhu 1 Haofei Yu 1 Tao Feng 1 Muhan Zhang 2 Mostofa Patwary 3 Jiaxuan You 1,3 1 Universit…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2510.23595v3.md` · `raw/arxiv/2510.23595v3.fulltext.md`
