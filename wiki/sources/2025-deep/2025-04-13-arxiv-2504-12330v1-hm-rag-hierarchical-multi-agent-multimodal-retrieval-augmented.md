---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation"
authors: Pei Liu, Xin Liu, Ruoyu Yao, Junming Liu et al.
url: https://arxiv.org/abs/2504.12330v1
date: 2025-04-13
citationCount: 55
influentialCitationCount: 2
velocity: 3.85
ingested: 2026-06-22
tags: [agentic-rag, multi-agent-systems, agent-evaluation, governance-gap, agentic-ai, arxiv, 2025, cited]
---

# HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation

**arXiv [2504.12330v1](https://arxiv.org/abs/2504.12330v1)** · 2025-04-13 · **55 citations** (2 influential · 3.85/mo) · Pei Liu, Xin Liu, Ruoyu Yao, Junming Liu et al.

## Abstract
While Retrieval-Augmented Generation (RAG) augments Large Language Models (LLMs) with external knowledge, conventional single-agent RAG remains fundamentally limited in resolving complex queries demanding coordinated reasoning across heterogeneous data ecosystems. We present HM-RAG, a novel Hierarchical Multi-agent Multimodal RAG framework that pioneers collaborative intelligence for dynamic knowledge synthesis across structured, unstructured, and graph-based data. The framework is composed of three-tiered architecture with specialized agents: a Decomposition Agent that dissects complex queries into contextually coherent sub-tasks via semantic-aware query rewriting and schema-guided context augmentation; Multi-source Retrieval Agents that carry out parallel, modality-specific retrieval using plug-and-play modules designed for vector, graph, and web-based databases; and a Decision Agent that uses consistency voting to integrate multi-source answers and resolve discrepancies in retrieval results through Expert Model Refinement. This architecture attains comprehensive query understanding by combining textual, graph-relational, and web-derived evidence, resulting in a remarkable 12.95% improvement in answer accuracy and a 3.56% boost in question classification accuracy over baseline RAG systems on the ScienceQA and CrisisMMD benchmarks. Notably, HM-RAG establishes state-of-the-art results in zero-shot settings on both datasets. Its modular architecture ensures seamless integration of new data modalities while maintaining strict data governance, marking a significant advancement in addressing the critical challenges of multimodal reasoning and knowledge synthesis in RAG systems. Code is available at https://github.com/ocean-luna/HMRAG.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Retrieval-Augmented Generation 2.2 Agents in RAG 3 Methodology 3.1 Multimodal Knowledge Pre-Processing 3.1.1 Multimodal Textual Knowledge Generation 3.1.2 Multimodal Knowledge Graphs Construction 3.2 Decomposition Agent for Multi-intent Queries 3.3 Multi-source Plug-and-Play Retrieval Agents 3.3.1 Vector-based Retrieval Agent for Fine-Grained Information 3.3.2 Graph-based Retrieval Agent for Relational Information 3.3.3 Web-based Retrieval Agent for Real-Time Information 3.4 Decision Agent for Multi-answer Refinement 4 Experiments 4.1 Experimental Setup 4.2 Main Results 4.2.1 Results on ScienceQA 4.2.2 Results on CrisisMMD 4.3 Qualitative Analysis 4.4 Ablation Studies 5 Conclusion A Predicted Examples HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation Pei Liu 1,2 , Xin Liu 2 , Ruoyu Yao 2 , Junming Liu 1 , Siyuan Meng 1 , Ding Wang 1∗ , Jun Ma 23∗ 1 Shanghai Artificial Intelligence Laboratory 2 The Hong Kong University of Science and Technology (Guang…

**Method / approach.** Methodology 3.1 Multimodal Knowledge Pre-Processing 3.1.1 Multimodal Textual Knowledge Generation 3.1.2 Multimodal Knowledge Graphs Construction 3.2 Decomposition Agent for Multi-intent Queries 3.3 Multi-source Plug-and-Play Retrieval Agents 3.3.1 Vector-based Retrieval Agent for Fine-Grained Information 3.3.2 Graph-based Retrieval Agent for Relational Information 3.3.3 Web-based Retrieval Agent for Real-Time Information 3.4 Decision Agent for Multi-answer Refinement 4 Experiments 4.1 Experimental Setup 4.2 Main Results 4.2.1 Results on ScienceQA 4.2.2 Results on CrisisMMD 4.3 Qualitative Analysis 4.4 Ablation Studies 5 Conclusion A Predicted Examples HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation Pei Liu 1,2 , Xin Liu 2 , Ruoyu Yao 2 , Junming Liu 1 , Siyuan Meng 1 , Ding Wang 1∗ , Jun Ma 23∗ 1 Shanghai Artificial Intelligence Laboratory 2 The Hong Kong University of Science and Technology (…

**Results.** Experiments 4.1 Experimental Setup 4.2 Main Results 4.2.1 Results on ScienceQA 4.2.2 Results on CrisisMMD 4.3 Qualitative Analysis 4.4 Ablation Studies 5 Conclusion A Predicted Examples HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation Pei Liu 1,2 , Xin Liu 2 , Ruoyu Yao 2 , Junming Liu 1 , Siyuan Meng 1 , Ding Wang 1∗ , Jun Ma 23∗ 1 Shanghai Artificial Intelligence Laboratory 2 The Hong Kong University of Science and Technology (Guangzhou) 3 The Hong Kong University of Science and Technology pliu061@connect.hkust-gz.edu.cn wangding@pjlab.org.cn jun.ma@ust.hk (2018) Abstract. While Retrieval-Augmented Generation (RAG) augments Large Language Models (LLMs) with external knowledge, conventional single-agent RAG remains fundamentally limited in resolving complex queries demanding coordinated reasoning across heterogeneous data ecosystems. We present HM-RAG, a novel…

**Conclusion.** Conclusion A Predicted Examples HM-RAG: Hierarchical Multi-Agent Multimodal Retrieval Augmented Generation Pei Liu 1,2 , Xin Liu 2 , Ruoyu Yao 2 , Junming Liu 1 , Siyuan Meng 1 , Ding Wang 1∗ , Jun Ma 23∗ 1 Shanghai Artificial Intelligence Laboratory 2 The Hong Kong University of Science and Technology (Guangzhou) 3 The Hong Kong University of Science and Technology pliu061@connect.hkust-gz.edu.cn wangding@pjlab.org.cn jun.ma@ust.hk (2018) Abstract. While Retrieval-Augmented Generation (RAG) augments Large Language Models (LLMs) with external knowledge, conventional single-agent RAG remains fundamentally limited in resolving complex queries demanding coordinated reasoning across heterogeneous data ecosystems. We…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.12330v1.md` · `raw/arxiv/2504.12330v1.fulltext.md`
