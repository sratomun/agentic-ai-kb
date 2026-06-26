---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepAnalyze: Agentic Large Language Models for Autonomous Data Science"
authors: Shaolei Zhang, Ju Fan, Meihao Fan, Guoliang Li et al.
url: https://arxiv.org/abs/2510.16872v1
date: 2025-10-19
citationCount: 35
influentialCitationCount: 3
velocity: 4.33
ingested: 2026-06-22
tags: [science-agents, agentic-ai, arxiv, 2025, cited]
---

# DeepAnalyze: Agentic Large Language Models for Autonomous Data Science

**arXiv [2510.16872v1](https://arxiv.org/abs/2510.16872v1)** · 2025-10-19 · **35 citations** (3 influential · 4.33/mo) · Shaolei Zhang, Ju Fan, Meihao Fan, Guoliang Li et al.

## Abstract
Autonomous data science, from raw data sources to analyst-grade deep research reports, has been a long-standing challenge, and is now becoming feasible with the emergence of powerful large language models (LLMs). Recent workflow-based data agents have shown promising results on specific data tasks but remain fundamentally limited in achieving fully autonomous data science due to their reliance on predefined workflows. In this paper, we introduce DeepAnalyze-8B, the first agentic LLM designed for autonomous data science, capable of automatically completing the end-toend pipeline from data sources to analyst-grade deep research reports. To tackle high-complexity data science tasks, we propose a curriculum-based agentic training paradigm that emulates the learning trajectory of human data scientists, enabling LLMs to progressively acquire and integrate multiple capabilities in real-world environments. We also introduce a data-grounded trajectory synthesis framework that constructs high-quality training data. Through agentic training, DeepAnalyze learns to perform a broad spectrum of data tasks, ranging from data question answering and specialized analytical tasks to open-ended data research. Experiments demonstrate that, with only 8B parameters, DeepAnalyze outperforms previous workflow-based agents built on most advanced proprietary LLMs. The model, code, and training data of DeepAnalyze are open-sourced, paving the way toward autonomous data science.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 DeepAnalyze 3.1 Architecture 3.2 Curriculum-based Agentic Training 3.3 Data-grounded Trajectory Synthesis 3.4 DataScience-Instruct-500K 4 Experiments 4.1 Benchmarks 4.2 Experimental Setup 4.3 Main Results 5 Analysis 5.1 Ablation on DeepAnalyze’s Actions 5.2 Superiority of Curriculum-based Agentic Training 5.3 Advantage of Reasoning Trajectory Synthesis 6 Conclusion and Future Work A Construction of DABStep-Research Benchmark B Keyword-guided Reasoning Trajectory Synthesis C Cases DeepAnalyze: Agentic Large Language Models for Autonomous Data Science Shaolei Zhang Ju Fan Meihao Fan Guoliang Li Xiaoyong Du Abstract Autonomous data science, from raw data sources to analyst-grade deep research reports, has been a long-standing challenge, and is now becoming feasible with the emergence of powerful large language models (LLMs). Recent workflow-based data agents have shown promising results on specific data tasks but remain fundamentally limited in achieving fully autonomous data science due to th…

**Method / approach.** methods from workflow-based agents to a trainable agentic model that learns to autonomously perform data science tasks in real-world environments. However, applying agentic training to this domain presents two key challenges: reward sparsity and trajectory scarcity . On the one hand, the inherent complexity of data science tasks makes it difficult for foundation LLMs to complete tasks successfully during the early stages of training. This leads to severe reward sparsity, i.e., a lack of positive reinforcement signals, which can hinder or even collapse the entire agentic training process. On the other hand, the scarcity of long-chain problem-solving trajectories in data science provides insufficient guidance for LLMs to explore the solution space effectively, resulting in inefficient, blind trial-and-error exploration without meaningful intermediate supervision. To address these challenges, we introduce DeepAnalyze, an agentic LLM designed for autonomous data science. As illustrated…

**Results.** Experiments 4.1 Benchmarks 4.2 Experimental Setup 4.3 Main Results 5 Analysis 5.1 Ablation on DeepAnalyze’s Actions 5.2 Superiority of Curriculum-based Agentic Training 5.3 Advantage of Reasoning Trajectory Synthesis 6 Conclusion and Future Work A Construction of DABStep-Research Benchmark B Keyword-guided Reasoning Trajectory Synthesis C Cases DeepAnalyze: Agentic Large Language Models for Autonomous Data Science Shaolei Zhang Ju Fan Meihao Fan Guoliang Li Xiaoyong Du Abstract Autonomous data science, from raw data sources to analyst-grade deep research reports, has been a long-standing challenge, and is now becoming feasible with the emergence of powerful large language models (LLMs). Recent workflow-based data agents have shown promising results on specific data tasks but remain fundamentally limited in achieving fully autonomous data science due to their reliance on predefined workflows.…

**Conclusion.** Conclusion and Future Work A Construction of DABStep-Research Benchmark B Keyword-guided Reasoning Trajectory Synthesis C Cases DeepAnalyze: Agentic Large Language Models for Autonomous Data Science Shaolei Zhang Ju Fan Meihao Fan Guoliang Li Xiaoyong Du Abstract Autonomous data science, from raw data sources to analyst-grade deep research reports, has been a long-standing challenge, and is now becoming feasible with the emergence of powerful large language models (LLMs). Recent workflow-based data agents have shown promising results on specific data tasks but remain fundamentally limited in achieving fully autonomous data science due to their reliance on predefined workflows. In this paper, we introduce DeepAnalyze-…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2510.16872v1.md` · `raw/arxiv/2510.16872v1.fulltext.md`
