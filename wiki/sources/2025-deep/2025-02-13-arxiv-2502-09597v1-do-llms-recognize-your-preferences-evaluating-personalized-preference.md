---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Do LLMs Recognize Your Preferences? Evaluating Personalized Preference Following in LLMs"
authors: Siyan Zhao, Mingyi Hong, Yang Liu, Devamanyu Hazarika et al.
url: https://arxiv.org/abs/2502.09597v1
date: 2025-02-13
citationCount: 107
influentialCitationCount: 15
velocity: 6.59
ingested: 2026-06-22
tags: [agentic-rag, agent-evaluation, arxiv, 2025, cited]
---

# Do LLMs Recognize Your Preferences? Evaluating Personalized Preference Following in LLMs

**arXiv [2502.09597v1](https://arxiv.org/abs/2502.09597v1)** · 2025-02-13 · **107 citations** (15 influential · 6.59/mo) · Siyan Zhao, Mingyi Hong, Yang Liu, Devamanyu Hazarika et al.

## Abstract
Large Language Models (LLMs) are increasingly used as chatbots, yet their ability to personalize responses to user preferences remains limited. We introduce PrefEval, a benchmark for evaluating LLMs' ability to infer, memorize and adhere to user preferences in a long-context conversational setting. PrefEval comprises 3,000 manually curated user preference and query pairs spanning 20 topics. PrefEval contains user personalization or preference information in both explicit and implicit forms, and evaluates LLM performance using a generation and a classification task. With PrefEval, we evaluated the aforementioned preference following capabilities of 10 open-source and proprietary LLMs in multi-session conversations with varying context lengths up to 100k tokens. We benchmark with various prompting, iterative feedback, and retrieval-augmented generation methods. Our benchmarking effort reveals that state-of-the-art LLMs face significant challenges in proactively following users' preferences during conversations. In particular, in zero-shot settings, preference following accuracy falls below 10% at merely 10 turns (~3k tokens) across most evaluated models. Even with advanced prompting and retrieval methods, preference following still deteriorates in long-context conversations. Furthermore, we show that fine-tuning on PrefEval significantly improves performance. We believe PrefEval serves as a valuable resource for measuring, understanding, and enhancing LLMs' preference following abilities, paving the way for personalized conversational agents. Our code and dataset are available at https://prefeval.github.io/.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 The PrefEval Dataset 2.1 Problem Formulation 2.2 PrefEval Statistics 2.3 Preference Forms 2.4 Multi-Session Conversational Context 2.5 Task Types and Evaluation Protocols Generation Task and LLM-based Evaluators. Classification Task and MCQ Accuracy. Practical Guide to Using PrefEval . 3 Experiments 3.1 Models and Methods 3.2 Explicit Preference Following 3.3 Implicit Preference Following 3.4 Classification Task 3.5 Error Type Analysis 3.6 Dynamic Preference Following 3.7 Finetuning on PrefEval To Improve Preference Following 4 Related Work 5 Conclusion 6 Reproducibility Statement 7 Ethics Statement A Appendix A.1 Limitation A.2 Detailed Related Works A.3 Model version A.4 Methods Description Zero-shot: Reminder: Self-Critic: Few-Shot Chain-of-Thought (CoT): Retrieval-Augmented Generation (RAG): A.5 Classification Task Correlation Plot A.6 Proprietary LLMs performance comparison A.7 RAG method ablation and analysis A.8 Cross-Topic Performances A.9 Examples of Data in PrefEval…

**Method / approach.** Methods 3.2 Explicit Preference Following 3.3 Implicit Preference Following 3.4 Classification Task 3.5 Error Type Analysis 3.6 Dynamic Preference Following 3.7 Finetuning on PrefEval To Improve Preference Following 4 Related Work 5 Conclusion 6 Reproducibility Statement 7 Ethics Statement A Appendix A.1 Limitation A.2 Detailed Related Works A.3 Model version A.4 Methods Description Zero-shot: Reminder: Self-Critic: Few-Shot Chain-of-Thought (CoT): Retrieval-Augmented Generation (RAG): A.5 Classification Task Correlation Plot A.6 Proprietary LLMs performance comparison A.7 RAG method ablation and analysis A.8 Cross-Topic Performances A.9 Examples of Data in PrefEval A.10 Absolute Error Types Trends A.11 Prompts used for LLM-based evaluation for 4 error types’s binary checks A.12 Attention Score Visualization Analysis A.12.1 Attention Score Changes After Supervised Fine-tuning A.12.2 Attention Score Analysis Acro…

**Results.** Experiments 3.1 Models and Methods 3.2 Explicit Preference Following 3.3 Implicit Preference Following 3.4 Classification Task 3.5 Error Type Analysis 3.6 Dynamic Preference Following 3.7 Finetuning on PrefEval To Improve Preference Following 4 Related Work 5 Conclusion 6 Reproducibility Statement 7 Ethics Statement A Appendix A.1 Limitation A.2 Detailed Related Works A.3 Model version A.4 Methods Description Zero-shot: Reminder: Self-Critic: Few-Shot Chain-of-Thought (CoT): Retrieval-Augmented Generation (RAG): A.5 Classification Task Correlation Plot A.6 Proprietary LLMs performance comparison A.7 RAG method ablation and analysis A.8 Cross-Topic Performances A.9 Examples of Data in PrefEval A.10 Absolute Error Types Trends A.11 Prompts used for LLM-based evaluation for 4 error types’s binary checks A.12 Attention Score Visualization Analysis A.12.1 Attention S…

**Conclusion.** Conclusion 6 Reproducibility Statement 7 Ethics Statement A Appendix A.1 Limitation A.2 Detailed Related Works A.3 Model version A.4 Methods Description Zero-shot: Reminder: Self-Critic: Few-Shot Chain-of-Thought (CoT): Retrieval-Augmented Generation (RAG): A.5 Classification Task Correlation Plot A.6 Proprietary LLMs performance comparison A.7 RAG method ablation and analysis A.8 Cross-Topic Performances A.9 Examples of Data in PrefEval A.10 Absolute Error Types Trends A.11 Prompts used for LLM-based evaluation for 4 error types’s binary checks A.12 Attention Score Visualization Analysis A.12.1 Attention Score Changes After Supervised Fine-tuning A.12.2 Attention Score Analysis Acros…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2502.09597v1.md` · `raw/arxiv/2502.09597v1.fulltext.md`
