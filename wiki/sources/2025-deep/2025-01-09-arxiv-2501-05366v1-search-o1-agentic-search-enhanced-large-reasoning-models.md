---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Search-o1: Agentic Search-Enhanced Large Reasoning Models"
authors: Xiaoxi Li, Guanting Dong, Jiajie Jin, Yuyao Zhang et al.
url: https://arxiv.org/abs/2501.05366v1
date: 2025-01-09
citationCount: 429
influentialCitationCount: 45
velocity: 24.69
ingested: 2026-06-22
tags: [agent-reliability, agentic-rl, agentic-rag, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Search-o1: Agentic Search-Enhanced Large Reasoning Models

**arXiv [2501.05366v1](https://arxiv.org/abs/2501.05366v1)** · 2025-01-09 · **429 citations** (45 influential · 24.69/mo) · Xiaoxi Li, Guanting Dong, Jiajie Jin, Yuyao Zhang et al.

**Significance:** Popularized interleaving agentic search with long reasoning — a backbone idea for agentic RAG.

## Abstract
Large reasoning models (LRMs) like OpenAI-o1 have demonstrated impressive long stepwise reasoning capabilities through large-scale reinforcement learning. However, their extended reasoning processes often suffer from knowledge insufficiency, leading to frequent uncertainties and potential errors. To address this limitation, we introduce \textbf{Search-o1}, a framework that enhances LRMs with an agentic retrieval-augmented generation (RAG) mechanism and a Reason-in-Documents module for refining retrieved documents. Search-o1 integrates an agentic search workflow into the reasoning process, enabling dynamic retrieval of external knowledge when LRMs encounter uncertain knowledge points. Additionally, due to the verbose nature of retrieved documents, we design a separate Reason-in-Documents module to deeply analyze the retrieved information before injecting it into the reasoning chain, minimizing noise and preserving coherent reasoning flow. Extensive experiments on complex reasoning tasks in science, mathematics, and coding, as well as six open-domain QA benchmarks, demonstrate the strong performance of Search-o1. This approach enhances the trustworthiness and applicability of LRMs in complex reasoning tasks, paving the way for more reliable and versatile intelligent systems. The code is available at \url{https://github.com/sunnynexus/Search-o1}.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Large Reasoning Models. Retrieval-Augmented Generation. 3 Methodology 3.1 Problem Formulation 3.2 Overview of the Search-o1 Framework 3.3 Agentic Retrieval-Augmented Generation Mechanism 3.4 Knowledge Refinement via Reason-in-Documents 3.5 Search-o1 Inference Process Inference Logic for a Single Question. Batch Inference Mechanism. 4 Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Challenging Reasoning Tasks Main Results. Scaling Analysis on Number of Retrieved Documents. Comparison with Human Experts. 4.5 Results on Open-Domain QA Tasks 5 Conclusion A Instruction Templates A.1 Instructions for Search-o1 A.2 Instructions for Standard RAG A.3 Instructions for RAG Agent A.4 Task-Specific Instructions A.4.1 Open-Domain QA Tasks Instruction A.4.2 Math Tasks Instruction A.4.3 Multi-choice Tasks Instruction A.4.4 Code Tasks Instruction A.5 Additional Notes B Case Study {CJK} UTF8gbsn Search-o1: Agentic Search-Enhanced…

**Method / approach.** Methodology 3.1 Problem Formulation 3.2 Overview of the Search-o1 Framework 3.3 Agentic Retrieval-Augmented Generation Mechanism 3.4 Knowledge Refinement via Reason-in-Documents 3.5 Search-o1 Inference Process Inference Logic for a Single Question. Batch Inference Mechanism. 4 Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Challenging Reasoning Tasks Main Results. Scaling Analysis on Number of Retrieved Documents. Comparison with Human Experts. 4.5 Results on Open-Domain QA Tasks 5 Conclusion A Instruction Templates A.1 Instructions for Search-o1 A.2 Instructions for Standard RAG A.3 Instructions for RAG Agent A.4 Task-Specific Instructions A.4.1 Open-Domain QA Tasks Instruction A.4.2 Math Tasks Instruction A.4.3 Multi-choice Tasks Instruction A.4.4 Code Tasks Instruction A.5 Additional Notes B Case Study {CJK} UTF8gbsn Search-o1: Agentic Search-Enhance…

**Results.** Experiments 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 4.4 Results on Challenging Reasoning Tasks Main Results. Scaling Analysis on Number of Retrieved Documents. Comparison with Human Experts. 4.5 Results on Open-Domain QA Tasks 5 Conclusion A Instruction Templates A.1 Instructions for Search-o1 A.2 Instructions for Standard RAG A.3 Instructions for RAG Agent A.4 Task-Specific Instructions A.4.1 Open-Domain QA Tasks Instruction A.4.2 Math Tasks Instruction A.4.3 Multi-choice Tasks Instruction A.4.4 Code Tasks Instruction A.5 Additional Notes B Case Study {CJK} UTF8gbsn Search-o1: Agentic Search-Enhanced Large Reasoning Models Xiaoxi Li 1 , Guanting Dong 1 , Jiajie Jin 1 , Yuyao Zhang 1 , Yujia Zhou 2 , Yutao Zhu 1 , Peitian Zhang 1 , Zhicheng Dou 1 1 Renmin University of China 2 Tsinghua University {xiaoxi_li, dou}@ruc.edu.cn Project…

**Conclusion.** Conclusion A Instruction Templates A.1 Instructions for Search-o1 A.2 Instructions for Standard RAG A.3 Instructions for RAG Agent A.4 Task-Specific Instructions A.4.1 Open-Domain QA Tasks Instruction A.4.2 Math Tasks Instruction A.4.3 Multi-choice Tasks Instruction A.4.4 Code Tasks Instruction A.5 Additional Notes B Case Study {CJK} UTF8gbsn Search-o1: Agentic Search-Enhanced Large Reasoning Models Xiaoxi Li 1 , Guanting Dong 1 , Jiajie Jin 1 , Yuyao Zhang 1 , Yujia Zhou 2 , Yutao Zhu 1 , Peitian Zhang 1 , Zhicheng Dou 1 1 Renmin University of China 2 Tsinghua University {xiaoxi_li, dou}@ruc.edu.cn Project Page: https://search-o1.github.io/ Correpsonding author. Abstract Large…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[search-o1]]
- **Raw:** `raw/arxiv/2501.05366v1.md` · `raw/arxiv/2501.05366v1.fulltext.md`
