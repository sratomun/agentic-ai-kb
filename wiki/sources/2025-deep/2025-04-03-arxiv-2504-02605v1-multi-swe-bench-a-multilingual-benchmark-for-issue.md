---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving"
authors: Daoguang Zan, Zhirong Huang, Wei Liu, Hanwu Chen et al.
url: https://arxiv.org/abs/2504.02605v1
date: 2025-04-03
citationCount: 120
influentialCitationCount: 13
velocity: 8.21
ingested: 2026-06-22
tags: [coding-agents, agent-reliability, agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving

**arXiv [2504.02605v1](https://arxiv.org/abs/2504.02605v1)** · 2025-04-03 · **120 citations** (13 influential · 8.21/mo) · Daoguang Zan, Zhirong Huang, Wei Liu, Hanwu Chen et al.

## Abstract
The task of issue resolving is to modify a codebase to generate a patch that addresses a given issue. However, existing benchmarks, such as SWE-bench, focus almost exclusively on Python, making them insufficient for evaluating Large Language Models (LLMs) across diverse software ecosystems. To address this, we introduce a multilingual issue-resolving benchmark, called Multi-SWE-bench, covering Java, TypeScript, JavaScript, Go, Rust, C, and C++. It includes a total of 1,632 high-quality instances, which were carefully annotated from 2,456 candidates by 68 expert annotators, ensuring that the benchmark can provide an accurate and reliable evaluation. Based on Multi-SWE-bench, we evaluate a series of state-of-the-art models using three representative methods (Agentless, SWE-agent, and OpenHands) and present a comprehensive analysis with key empirical insights. In addition, we launch a Multi-SWE-RL open-source community, aimed at building large-scale reinforcement learning (RL) training datasets for issue-resolving tasks. As an initial contribution, we release a set of 4,723 well-structured instances spanning seven programming languages, laying a solid foundation for RL research in this domain. More importantly, we open-source our entire data production pipeline, along with detailed tutorials, encouraging the open-source community to continuously contribute and expand the dataset. We envision our Multi-SWE-bench and the ever-growing Multi-SWE-RL community as catalysts for advancing RL toward its full potential, bringing us one step closer to the dawn of AGI.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Multi-SWE-bench 3.1 Benchmark Construction 3.1.1 Phase 1: Repository Selection 3.1.2 Phase 2: Pull Request Crawling 3.1.3 Phase 3: Environment Determination 3.1.4 Phase 4: Pull Request Filtering 3.1.5 Phase 5: Manual Verification 3.2 Features of Multi-SWE-bench 4 Multi-SWE-RL Open-Source Community 5 Experimental Setups 5.1 Evaluated LLMs and Methods 5.2 Evaluation Metrics 6 Experimental Results 6.1 Performance on Multi-SWE-bench 6.1.1 Performance across Programming Languages 6.1.2 Performance across Various Methods and LLMs 6.1.3 Performance across Different Repositories 6.2 Influencing Factors of Performance 6.2.1 Issue Type 6.2.2 Characteristics of Issue Description 6.2.3 Characteristics of Fix Patches 6.3 Case Study 6.4 Resource Consumption 6.5 Troubleshooting 7 Conclusions and Future Works Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving ByteDance Seed \tcb@lua@color tcbcolupper Leaderboard \tcb@lua@color tcbcolupper Benchmark \tcb@lua@color…

**Method / approach.** Methods 5.2 Evaluation Metrics 6 Experimental Results 6.1 Performance on Multi-SWE-bench 6.1.1 Performance across Programming Languages 6.1.2 Performance across Various Methods and LLMs 6.1.3 Performance across Different Repositories 6.2 Influencing Factors of Performance 6.2.1 Issue Type 6.2.2 Characteristics of Issue Description 6.2.3 Characteristics of Fix Patches 6.3 Case Study 6.4 Resource Consumption 6.5 Troubleshooting 7 Conclusions and Future Works Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving ByteDance Seed \tcb@lua@color tcbcolupper Leaderboard \tcb@lua@color tcbcolupper Benchmark \tcb@lua@color tcbcolupper RL Community \tcb@lua@color tcbcolupper GitHub Repo Abstract The task of issue resolving is to modify a codebase to generate a patch that addresses a given issue. However, existing benchmarks, such as SWE-bench, focus almost exclusively on Python, making them insufficient for eva…

**Results.** Experimental Setups 5.1 Evaluated LLMs and Methods 5.2 Evaluation Metrics 6 Experimental Results 6.1 Performance on Multi-SWE-bench 6.1.1 Performance across Programming Languages 6.1.2 Performance across Various Methods and LLMs 6.1.3 Performance across Different Repositories 6.2 Influencing Factors of Performance 6.2.1 Issue Type 6.2.2 Characteristics of Issue Description 6.2.3 Characteristics of Fix Patches 6.3 Case Study 6.4 Resource Consumption 6.5 Troubleshooting 7 Conclusions and Future Works Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving ByteDance Seed \tcb@lua@color tcbcolupper Leaderboard \tcb@lua@color tcbcolupper Benchmark \tcb@lua@color tcbcolupper RL Community \tcb@lua@color tcbcolupper GitHub Repo Abstract The task of issue resolving is to modify a codebase to generate a patch that addresses a given issue. However, existing ben…

**Conclusion.** Conclusions and Future Works Multi-SWE-bench: A Multilingual Benchmark for Issue Resolving ByteDance Seed \tcb@lua@color tcbcolupper Leaderboard \tcb@lua@color tcbcolupper Benchmark \tcb@lua@color tcbcolupper RL Community \tcb@lua@color tcbcolupper GitHub Repo Abstract The task of issue resolving is to modify a codebase to generate a patch that addresses a given issue. However, existing benchmarks, such as SWE-bench, focus almost exclusively on Python, making them insufficient for evaluating Large Language Models (LLMs) across diverse software ecosystems. To address this, we introduce a multilingual issue-resolving benchmark, called Multi-SWE-bench, covering Java, TypeScript, JavaScript, Go, Rust, C,…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2504.02605v1.md` · `raw/arxiv/2504.02605v1.fulltext.md`
