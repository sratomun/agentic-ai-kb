---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Consistently Simulating Human Personas with Multi-Turn Reinforcement Learning"
authors: Marwa Abdulhai, Ryan Cheng, Donovan Clay, Tim Althoff et al.
url: https://arxiv.org/abs/2511.00222v1
date: 2025-10-31
citationCount: 32
influentialCitationCount: 3
velocity: 4.16
ingested: 2026-06-22
tags: [clinical-agents, agentic-rl, arxiv, 2025, cited]
---

# Consistently Simulating Human Personas with Multi-Turn Reinforcement Learning

**arXiv [2511.00222v1](https://arxiv.org/abs/2511.00222v1)** · 2025-10-31 · **32 citations** (3 influential · 4.16/mo) · Marwa Abdulhai, Ryan Cheng, Donovan Clay, Tim Althoff et al.

## Abstract
Large Language Models (LLMs) are increasingly used to simulate human users in interactive settings such as therapy, education, and social role-play. While these simulations enable scalable training and evaluation of AI agents, off-the-shelf LLMs often drift from their assigned personas, contradict earlier statements, or abandon role-appropriate behavior. We introduce a unified framework for evaluating and improving persona consistency in LLM-generated dialogue. We define three automatic metrics: prompt-to-line consistency, line-to-line consistency, and Q&A consistency, that capture different types of persona drift and validate each against human annotations. Using these metrics as reward signals, we apply multi-turn reinforcement learning to fine-tune LLMs for three user roles: a patient, a student, and a social chat partner. Our method reduces inconsistency by over 55%, resulting in more coherent and faithful simulated users.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 LLMs as Human Simulators 2.2 Consistency in LLMs 2.3 Techniques for Improving Consistency 3 Defining, Evaluating and Improving Consistency for LLMs 3.1 LLM-as-a-Judge for Consistency Scoring 3.2 Metrics for Measuring Consistency Prompt-to-Line Consistency. Line-to-Line Consistency. Q A Consistency. 3.3 Data Generation 3.4 Multi-Turn Reinforcement Learning for Consistent Dialogue 3.5 Evaluation After Fine-Tuning 4 Experimental Methodology 4.1 Dialogue Tasks 4.2 Experimental Questions Q1: Do our proposed consistency metrics align with human judgments? Q2: How consistent are different LLM-generated dialogues across tasks? Q3: Can we increase consistency of dialogue through multi-turn RL fine-tuning? 5 Results Q1. Human Evaluation. Q2. Consistency of LLM-generated dialogue. Q3. Multi-turn RL for Consistency. 6 Limitations 7 Conclusion 8 Ethics Statement 9 Acknowledgment 10 Appendix 10.1 Measuring Consistency Consistency metrics. Prompt-to-line consistency. Line-to-l…

**Method / approach.** Methodology 4.1 Dialogue Tasks 4.2 Experimental Questions Q1: Do our proposed consistency metrics align with human judgments? Q2: How consistent are different LLM-generated dialogues across tasks? Q3: Can we increase consistency of dialogue through multi-turn RL fine-tuning? 5 Results Q1. Human Evaluation. Q2. Consistency of LLM-generated dialogue. Q3. Multi-turn RL for Consistency. 6 Limitations 7 Conclusion 8 Ethics Statement 9 Acknowledgment 10 Appendix 10.1 Measuring Consistency Consistency metrics. Prompt-to-line consistency. Line-to-line consistency. Q A Consistency. Question Generation. Question Answering. Answer Grading. 10.2 Task Details Open-Ended Conversation. Open-Ended Conversation Example Conversations. Education. Education Example Conversations. Mental Health. Mental Health Example Conversations. 10.3 Training Details Compute Requirements. 10.4 Human Evaluation Human Annotators.…

**Results.** Experimental Methodology 4.1 Dialogue Tasks 4.2 Experimental Questions Q1: Do our proposed consistency metrics align with human judgments? Q2: How consistent are different LLM-generated dialogues across tasks? Q3: Can we increase consistency of dialogue through multi-turn RL fine-tuning? 5 Results Q1. Human Evaluation. Q2. Consistency of LLM-generated dialogue. Q3. Multi-turn RL for Consistency. 6 Limitations 7 Conclusion 8 Ethics Statement 9 Acknowledgment 10 Appendix 10.1 Measuring Consistency Consistency metrics. Prompt-to-line consistency. Line-to-line consistency. Q A Consistency. Question Generation. Question Answering. Answer Grading. 10.2 Task Details Open-Ended Conversation. Open-Ended Conversation Example Conversations. Education. Education Example Conversations. Mental Health. Mental Health Example Conversations. 10.3 Training Details Compute R…

**Conclusion.** Conclusion 8 Ethics Statement 9 Acknowledgment 10 Appendix 10.1 Measuring Consistency Consistency metrics. Prompt-to-line consistency. Line-to-line consistency. Q A Consistency. Question Generation. Question Answering. Answer Grading. 10.2 Task Details Open-Ended Conversation. Open-Ended Conversation Example Conversations. Education. Education Example Conversations. Mental Health. Mental Health Example Conversations. 10.3 Training Details Compute Requirements. 10.4 Human Evaluation Human Annotators. 10.5 Results Consistency over dialogue length before fine-tuning (in support of Q2). Consistency of Larger Models (in support of Q2) Consistency over dialogue length after fine…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rl|Agentic RL]]
- **Raw:** `raw/arxiv/2511.00222v1.md` · `raw/arxiv/2511.00222v1.fulltext.md`
