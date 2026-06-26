---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "RepoAudit: An Autonomous LLM-Agent for Repository-Level Code Auditing"
authors: Jinyao Guo, Chengpeng Wang, Xiangzhe Xu, Zian Su et al.
url: https://arxiv.org/abs/2501.18160v3
date: 2025-01-30
citationCount: 56
influentialCitationCount: 9
velocity: 3.36
ingested: 2026-06-22
tags: [coding-agents, agent-memory, agent-evaluation, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# RepoAudit: An Autonomous LLM-Agent for Repository-Level Code Auditing

**arXiv [2501.18160v3](https://arxiv.org/abs/2501.18160v3)** · 2025-01-30 · **56 citations** (9 influential · 3.36/mo) · Jinyao Guo, Chengpeng Wang, Xiangzhe Xu, Zian Su et al.

## Abstract
Code auditing is the process of reviewing code with the aim of identifying bugs. Large Language Models (LLMs) have demonstrated promising capabilities for this task without requiring compilation, while also supporting user-friendly customization. However, auditing a code repository with LLMs poses significant challenges: limited context windows and hallucinations can degrade the quality of bug reports, and analyzing large-scale repositories incurs substantial time and token costs, hindering efficiency and scalability. This work introduces an LLM-based agent, RepoAudit, designed to perform autonomous repository-level code auditing. Equipped with agent memory, RepoAudit explores the codebase on demand by analyzing data-flow facts along feasible program paths within individual functions. It further incorporates a validator module to mitigate hallucinations by verifying data-flow facts and checking the satisfiability of path conditions associated with potential bugs, thereby reducing false positives. RepoAudit detects 40 true bugs across 15 real-world benchmark projects with a precision of 78.43%, requiring on average only 0.44 hours and $2.54 per project. Also, it detects 185 new bugs in high-profile projects, among which 174 have been confirmed or fixed. We have open-sourced RepoAudit at https://github.com/PurCL/RepoAudit.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Preliminaries 2.1 Auditing Entails Path-Sensitive Reasoning on Complex Graphs 2.2 LLMs’ Inadequacy 2.3 Intrinsic Strengths of LLMs 2.3.1 Program Abstraction 2.3.2 Pointer Handling 2.3.3 Feasible Program Path Exploration 3 RepoAudit 3.1 Initiator 3.2 Explorer 3.2.1 Analyzing Individual Functions 3.2.2 Selecting Functions for Exploration 3.2.3 Generating Bug Report Candidates 3.3 Validator 4 Evaluation 4.1 Bug Types and Dataset 4.2 Evaluation Results 4.3 Limitations and Future Works 5 Related Work 6 Conclusion A Comparison with LLM-driven Detectors B Comparison with Industrial Bug Detectors C Ablation Study D Evaluation with More Reasoning Models E Evaluation with Different Temperatures F Examples of False Positive/Negative RepoAudit : An Autonomous LLM-Agent for Repository-Level Code Auditing Jinyao Guo ∗ Chengpeng Wang ∗ Xiangzhe Xu Zian Su Xiangyu Zhang Abstract Code auditing is the process of reviewing code with the aim of identifying bugs. Large Language Models (LLMs) have de…

**Method / approach.** methodology similar to a recent study (Fang et al., 2024 ) . This is a controlled experiment because, in practice, we cannot guarantee knowledge of the comprehensive set of functions associated with a bug. The model exhibited substantial hallucinations, reporting that almost all the dereferenced pointers have null values. Even if we improve the prompts by offering several few-shot examples and explanations on how a null pointer dereference bug occurs, the model still hallucinates, producing false positives and incorrect explanations. More numerical results can be found in Appendix A . 2.3 Intrinsic Strengths of LLMs On the bright side, we observe that LLMs can effectively perform basic analyses when the scope is limited. This capability enables us to surpass traditional program analysis methods, which require compilation and struggle to scale efficiently. Specifically, we identify several primitive abilities critical for auditing: program abstraction , pointer handling , and…

**Results.** experiments in Section 2.2 . In addition, detecting many types of bugs requires reasoning about properties along specific program paths. For instance, a memory leak occurs when allocated memory is not freed along some program path. Detecting such so-called path-sensitive bugs (Shi et al., 2018a ) necessitates unfolding the program’s graph structure into individual paths and analyzing these paths one by one. However, this leads to the well-known path explosion problem, as the number of paths grows exponentially with the number of statements. Hence, direct prompting is akin to presenting a large project on an enormous screen and expecting a human auditor to identify bugs along complex and lengthy paths solely by reading and interpreting the code—a task highly unlikely to succeed. Human Auditing. In practice, human auditors do not operate in such a manner. As revealed by existing cognitive science literature (Anicic et al., 2012…

**Conclusion.** Conclusion A Comparison with LLM-driven Detectors B Comparison with Industrial Bug Detectors C Ablation Study D Evaluation with More Reasoning Models E Evaluation with Different Temperatures F Examples of False Positive/Negative RepoAudit : An Autonomous LLM-Agent for Repository-Level Code Auditing Jinyao Guo ∗ Chengpeng Wang ∗ Xiangzhe Xu Zian Su Xiangyu Zhang Abstract Code auditing is the process of reviewing code with the aim of identifying bugs. Large Language Models (LLMs) have demonstrated promising capabilities for this task without requiring compilation, while also supporting user-friendly customization. However, auditing a code repository with LLMs poses significant challenges: limited context window…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2501.18160v3.md` · `raw/arxiv/2501.18160v3.fulltext.md`
