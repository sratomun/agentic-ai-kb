---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions"
authors: Yuanzhe Hu, Yu Wang, Julian McAuley
url: https://arxiv.org/abs/2507.05257v3
date: 2025-07-07
citationCount: 117
influentialCitationCount: 14
velocity: 10.18
ingested: 2026-06-22
tags: [agentic-rag, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions

**arXiv [2507.05257v3](https://arxiv.org/abs/2507.05257v3)** · 2025-07-07 · **117 citations** (14 influential · 10.18/mo) · Yuanzhe Hu, Yu Wang, Julian McAuley

## Abstract
Recent benchmarks for Large Language Model (LLM) agents primarily focus on evaluating reasoning, planning, and execution capabilities, while another critical component-memory, encompassing how agents memorize, update, and retrieve long-term information-is under-evaluated due to the lack of benchmarks. We term agents with memory mechanisms as memory agents. In this paper, based on classic theories from memory science and cognitive science, we identify four core competencies essential for memory agents: accurate retrieval, test-time learning, long-range understanding, and selective forgetting. Existing benchmarks either rely on limited context lengths or are tailored for static, long-context settings like book-based QA, which do not reflect the interactive, multi-turn nature of memory agents that incrementally accumulate information. Moreover, no existing benchmarks cover all four competencies. We introduce MemoryAgentBench, a new benchmark specifically designed for memory agents. Our benchmark transforms existing long-context datasets and incorporates newly constructed datasets into a multi-turn format, effectively simulating the incremental information processing characteristic of memory agents. By carefully selecting and curating datasets, our benchmark provides comprehensive coverage of the four core memory competencies outlined above, thereby offering a systematic and challenging testbed for assessing memory quality. We evaluate a diverse set of memory agents, ranging from simple context-based and retrieval-augmented generation (RAG) systems to advanced agents with external memory modules and tool integration. Empirical results reveal that current methods fall short of mastering all four competencies, underscoring the need for further research into comprehensive memory mechanisms for LLM agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Benchmarks on Long-Context and Memory Benchmarks for Long-Context LLMs. Benchmarks for Retrieval-Augmented Generation. Benchmarks for Memory Agents 2.2 Agents with Memory Mechanisms 3 MemoryAgentBench 3.1 Dataset Preperation Datasets for Accurate Retrieval (AR) Datasets for Test-Time Learning (TTL) Datasets for Long Range Understanding (LRU) Datasets for Selective Forgetting (SF) 3.2 Different Categories of Memory Agents 3.3 Datasets and Agents Formulation Datasets Formulation Prompt Formulation and Interaction Protocol Agents Formulation 4 Experiments 4.1 Experimental Setup 4.2 Overall Performance Comparison 4.3 Analysis and Ablation Study 4.3.1 Ablation Study on Input Chunk Size 4.3.2 Ablation Study on Retrieval TopK 4.3.3 Ablation Study on Backbone Model 4.3.4 Validation of Dataset FactConsolidation 5 Conclusion References A The Use of Large Language Models (LLMs) B Details of Dataset B.1 Accurate Retrieval (AR) B.1.1 Definition of AR B.1.2 Details on AR…

**Method / approach.** Methodology I.2 Cost-Performance Results I.3 Key Insights J Strict Compute-Matched Comparative Experiments J.1 Experimental Setup K Prompt Design and Overwrite Policy Ablation Experiments K.1 Prompt Design Specification K.2 Overwrite Policy Ablation Experiments K.2.1 Ablation Results K.2.2 Key Insights L Supplementary Notes for LLM-as-a-Judge and Input Format L.1 Validity of LLM-as-a-Judge Evaluation L.2 Rationale for Chunked Input Format License: arXiv.org perpetual non-exclusive license arXiv:2507.05257v3 [cs.CL] 17 Mar 2026 Evaluating Memory in LLM Agents via Incremental Multi-Turn Interactions Yuanzhe Hu*†, Yu Wang*†, Julian McAuley University of California, San Diego {yuh127, yuw164, jmcauley}@ucsd.edu Datasets Source Code These authors contributed equally to this work.Joint corresponding authors. Abstract Recent benchmarks for Large Language Model (LLM) agents primarily focus on evaluating reasoning, planning, and ex…

**Results.** Experiments 4.1 Experimental Setup 4.2 Overall Performance Comparison 4.3 Analysis and Ablation Study 4.3.1 Ablation Study on Input Chunk Size 4.3.2 Ablation Study on Retrieval TopK 4.3.3 Ablation Study on Backbone Model 4.3.4 Validation of Dataset FactConsolidation 5 Conclusion References A The Use of Large Language Models (LLMs) B Details of Dataset B.1 Accurate Retrieval (AR) B.1.1 Definition of AR B.1.2 Details on AR datasets (1) Document Question Answering (2) LongMemEval (3) EventQA B.2 Test-time Learning (TTL) B.2.1 Definition of TTL B.2.2 Details on TTL datasets (1) Multi-Class Classification (MCC) (2) Recommendation (Recom.) B.3 Long-Range Understanding (LRU) B.3.1 Definition of LRU B.3.2 Details on LRU datasets B.4 Selective Forgetting (SF) B.4.1 Definition of SF B.4.2 Details on SF datasets B.5 Justification for competencies based on co…

**Conclusion.** Conclusion References A The Use of Large Language Models (LLMs) B Details of Dataset B.1 Accurate Retrieval (AR) B.1.1 Definition of AR B.1.2 Details on AR datasets (1) Document Question Answering (2) LongMemEval (3) EventQA B.2 Test-time Learning (TTL) B.2.1 Definition of TTL B.2.2 Details on TTL datasets (1) Multi-Class Classification (MCC) (2) Recommendation (Recom.) B.3 Long-Range Understanding (LRU) B.3.1 Definition of LRU B.3.2 Details on LRU datasets B.4 Selective Forgetting (SF) B.4.1 Definition of SF B.4.2 Details on SF datasets B.5 Justification for competencies based on cognitive science C Detailed Memory Agents Description C.1 Long-Context Agents C.2 R…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.05257v3.md` · `raw/arxiv/2507.05257v3.fulltext.md`
