---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-rebench: An Automated Pipeline for Task Collection and Decontaminated Evaluation of Software Engineering Agents"
authors: Ibragim Badertdinov, Alexander Golubev, Maksim Nekrashevich, Anton Shevtsov et al.
url: https://arxiv.org/abs/2505.20411v2
date: 2025-05-26
citationCount: 68
influentialCitationCount: 13
velocity: 5.28
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SWE-rebench: An Automated Pipeline for Task Collection and Decontaminated Evaluation of Software Engineering Agents

**arXiv [2505.20411v2](https://arxiv.org/abs/2505.20411v2)** · 2025-05-26 · **68 citations** (13 influential · 5.28/mo) · Ibragim Badertdinov, Alexander Golubev, Maksim Nekrashevich, Anton Shevtsov et al.

## Abstract
LLM-based agents have shown promising capabilities in a growing range of software engineering (SWE) tasks. However, advancing this field faces two critical challenges. First, high-quality training data is scarce, especially data that reflects real-world SWE scenarios, where agents must interact with development environments, execute code and adapt behavior based on the outcomes of their actions. Existing datasets are either limited to one-shot code generation or comprise small, manually curated collections of interactive tasks, lacking both scale and diversity. Second, the lack of fresh interactive SWE tasks affects evaluation of rapidly improving models, as static benchmarks quickly become outdated due to contamination issues. To address these limitations, we introduce a novel, automated, and scalable pipeline to continuously extract real-world interactive SWE tasks from diverse GitHub repositories. Using this pipeline, we construct SWE-rebench, a public dataset comprising over 21,000 interactive Python-based SWE tasks, suitable for reinforcement learning of SWE agents at scale. Additionally, we use continuous supply of fresh tasks collected using SWE-rebench methodology to build a contamination-free benchmark for agentic software engineering. We compare results of various LLMs on this benchmark to results on SWE-bench Verified and show that performance of some language models might be inflated due to contamination issues.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 An automated pipeline for collecting software engineering tasks 2.1 Preliminary task collection 2.2 Automated installation instructions configuration 2.3 Execution-based installation verification 2.4 Automated instance quality assessment 3 SWE-rebench benchmark 3.1 Challenges in SWE agent benchmarking 3.2 Principles of SWE-rebench 3.3 Result analysis 4 Discussion and limitations 5 Conclusion and future work A Related work Benchmarks for software engineering Training datasets for code generation B Automated dependency installation B.1 Identifying installation-related files B.2 Extracting installation recipe B.3 Example of LLM-generated installation recipe B.4 Updating installation recipe B.5 Failure modes during execution validation and mitigation strategies C Evaluation of automated installation recipe generation C.1 List of instances to validate automatic installation instruction extraction D Permissive licenses included in data collection E Example of a task instance with annotations F Comparison of…

**Method / approach.** methodology H Filtering criteria for the SWE-rebench benchmark subset I System prompt for agent runs J Evaluation details and experimental setup J.1 GPT-4.1 Trajectory Example J.2 Qwen2.5-32B Coder hallucination example K Dataset schema and fields L Data collection funnel and potential enhancements M SWE-rebench dataset statistics SWE-rebench: An Automated Pipeline for Task Collection and Decontaminated Evaluation of Software Engineering Agents Ibragim Badertdinov Nebius Alexander Golubev 1 1 footnotemark: 1 Nebius Maksim Nekrashevich Nebius Anton Shevtsov Nebius Simon Karasik Nebius Andrei Andriushchenko Nebius Maria Trofimova Nebius Daria Litvintseva Nebius Boris Yangel Nebius Equal contribution. Correspondence to ibragim-bad@nebius.com Abstract LLM-based agents have shown promising capabilities in a growing range of software engineering (SWE) tasks. However, advancing this field faces two critical challenges. Fir…

**Results.** experimental setup J.1 GPT-4.1 Trajectory Example J.2 Qwen2.5-32B Coder hallucination example K Dataset schema and fields L Data collection funnel and potential enhancements M SWE-rebench dataset statistics SWE-rebench: An Automated Pipeline for Task Collection and Decontaminated Evaluation of Software Engineering Agents Ibragim Badertdinov Nebius Alexander Golubev 1 1 footnotemark: 1 Nebius Maksim Nekrashevich Nebius Anton Shevtsov Nebius Simon Karasik Nebius Andrei Andriushchenko Nebius Maria Trofimova Nebius Daria Litvintseva Nebius Boris Yangel Nebius Equal contribution. Correspondence to ibragim-bad@nebius.com Abstract LLM-based agents have shown promising capabilities in a growing range of software engineering (SWE) tasks. However, advancing this field faces two critical challenges. First, high-quality training data is scarce, especially data that reflects real-world SW…

**Conclusion.** Conclusion and future work A Related work Benchmarks for software engineering Training datasets for code generation B Automated dependency installation B.1 Identifying installation-related files B.2 Extracting installation recipe B.3 Example of LLM-generated installation recipe B.4 Updating installation recipe B.5 Failure modes during execution validation and mitigation strategies C Evaluation of automated installation recipe generation C.1 List of instances to validate automatic installation instruction extraction D Permissive licenses included in data collection E Example of a task instance with annotations F Comparison of models for automatic task quality assessment G Refinements to the original S…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2505.20411v2.md` · `raw/arxiv/2505.20411v2.fulltext.md`
