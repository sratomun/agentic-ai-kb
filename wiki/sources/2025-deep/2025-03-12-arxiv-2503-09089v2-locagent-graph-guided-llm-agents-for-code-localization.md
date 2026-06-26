---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "LocAgent: Graph-Guided LLM Agents for Code Localization"
authors: Zhaoling Chen, Xiangru Tang, Gangda Deng, Fang Wu et al.
url: https://arxiv.org/abs/2503.09089v2
date: 2025-03-12
citationCount: 69
influentialCitationCount: 25
velocity: 4.5
ingested: 2026-06-22
tags: [agent-evaluation, arxiv, 2025, cited]
---

# LocAgent: Graph-Guided LLM Agents for Code Localization

**arXiv [2503.09089v2](https://arxiv.org/abs/2503.09089v2)** · 2025-03-12 · **69 citations** (25 influential · 4.5/mo) · Zhaoling Chen, Xiangru Tang, Gangda Deng, Fang Wu et al.

## Abstract
Code localization--identifying precisely where in a codebase changes need to be made--is a fundamental yet challenging task in software maintenance. Existing approaches struggle to efficiently navigate complex codebases when identifying relevant code sections. The challenge lies in bridging natural language problem descriptions with the appropriate code elements, often requiring reasoning across hierarchical structures and multiple dependencies. We introduce LocAgent, a framework that addresses code localization through graph-based representation. By parsing codebases into directed heterogeneous graphs, LocAgent creates a lightweight representation that captures code structures (files, classes, functions) and their dependencies (imports, invocations, inheritance), enabling LLM agents to effectively search and locate relevant entities through powerful multi-hop reasoning. Experimental results on real-world benchmarks demonstrate that our approach significantly enhances accuracy in code localization. Notably, our method with the fine-tuned Qwen-2.5-Coder-Instruct-32B model achieves comparable results to SOTA proprietary models at greatly reduced cost (approximately 86% reduction), reaching up to 92.7% accuracy on file-level localization while improving downstream GitHub issue resolution success rates by 12% for multiple attempts (Pass@10). Our code is available at https://github.com/gersteinlab/LocAgent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Traditional Retrieval-based Methods 2.2 LLM-based Generative Retrieval Methods 2.3 Graph-based Code Representation Methods 3 The LocAgent Framework 3.1 Graph-based Code Representation 3.2 Agent-guided Code Search 3.3 Open-source Model Fine-tuning 4 Loc-Bench : A New Benchmark for Code Localization 4.1 Revisiting Existing Benchmark 4.2 Dataset Construction 5 Experiments 5.1 Experimental Settings 5.2 Baselines 5.3 Evaluation Results on SWE-Bench-Lite 5.4 Fine-tuned Open-source Models 5.5 Efficiency Analysis 5.6 Ablation Study 5.7 Evaluation Results on Loc-Bench 5.8 Application: Better Localization Leads to More Solved GitHub Issues 6 Conclusion A LocAgent Design Details A.1 Tool Output Design A.1.1 Three-level format for SearchEntity output A.1.2 Tree-based Subgraph Formatting for TraverseGraph Output A.2 Implementation B Dataset construction and statistics B.1 Dataset construction details C Additional Experiments C.1 Implementation Details C.1.1 Baselines Implementa…

**Method / approach.** Methods 2.2 LLM-based Generative Retrieval Methods 2.3 Graph-based Code Representation Methods 3 The LocAgent Framework 3.1 Graph-based Code Representation 3.2 Agent-guided Code Search 3.3 Open-source Model Fine-tuning 4 Loc-Bench : A New Benchmark for Code Localization 4.1 Revisiting Existing Benchmark 4.2 Dataset Construction 5 Experiments 5.1 Experimental Settings 5.2 Baselines 5.3 Evaluation Results on SWE-Bench-Lite 5.4 Fine-tuned Open-source Models 5.5 Efficiency Analysis 5.6 Ablation Study 5.7 Evaluation Results on Loc-Bench 5.8 Application: Better Localization Leads to More Solved GitHub Issues 6 Conclusion A LocAgent Design Details A.1 Tool Output Design A.1.1 Three-level format for SearchEntity output A.1.2 Tree-based Subgraph Formatting for TraverseGraph Output A.2 Implementation B Dataset construction and statistics B.1 Dataset construction details C Additional Experiments C.1 Implementation Detai…

**Results.** Experiments 5.1 Experimental Settings 5.2 Baselines 5.3 Evaluation Results on SWE-Bench-Lite 5.4 Fine-tuned Open-source Models 5.5 Efficiency Analysis 5.6 Ablation Study 5.7 Evaluation Results on Loc-Bench 5.8 Application: Better Localization Leads to More Solved GitHub Issues 6 Conclusion A LocAgent Design Details A.1 Tool Output Design A.1.1 Three-level format for SearchEntity output A.1.2 Tree-based Subgraph Formatting for TraverseGraph Output A.2 Implementation B Dataset construction and statistics B.1 Dataset construction details C Additional Experiments C.1 Implementation Details C.1.1 Baselines Implementation C.1.2 Quantifying Task Difficulty Based on Code Graph Distance C.1.3 Training details. D Prompt LocAgent: Graph-Guided LLM Agents for Code Localization Zhaoling Chen ♠∗ , Xiangru Tang ♠ , Gangda Deng \vardiamondsuit ⁣ ∗ \vardiamondsuit {}^{\vardiamondsuit*} st…

**Conclusion.** Conclusion A LocAgent Design Details A.1 Tool Output Design A.1.1 Three-level format for SearchEntity output A.1.2 Tree-based Subgraph Formatting for TraverseGraph Output A.2 Implementation B Dataset construction and statistics B.1 Dataset construction details C Additional Experiments C.1 Implementation Details C.1.1 Baselines Implementation C.1.2 Quantifying Task Difficulty Based on Code Graph Distance C.1.3 Training details. D Prompt LocAgent: Graph-Guided LLM Agents for Code Localization Zhaoling Chen ♠∗ , Xiangru Tang ♠ , Gangda Deng \vardiamondsuit ⁣ ∗ \vardiamondsuit {}^{\vardiamondsuit*} start_FLOATSUPERSCRIPT ∗ end_FLOATSUPERSCRIPT , Fang Wu ♣ , Jialong Wu ♠ , Zhiwei Jiang, Viktor Prasan…

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2503.09089v2.md` · `raw/arxiv/2503.09089v2.fulltext.md`
