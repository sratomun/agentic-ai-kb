---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "ViDoRAG: Visual Document Retrieval-Augmented Generation via Dynamic Iterative Reasoning Agents"
authors: Qiuchen Wang, Ruixue Ding, Zehui Chen, Weiqi Wu et al.
url: https://arxiv.org/abs/2502.18017v2
date: 2025-02-25
citationCount: 57
influentialCitationCount: 8
velocity: 3.6
ingested: 2026-06-22
tags: [agentic-rag, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# ViDoRAG: Visual Document Retrieval-Augmented Generation via Dynamic Iterative Reasoning Agents

**arXiv [2502.18017v2](https://arxiv.org/abs/2502.18017v2)** · 2025-02-25 · **57 citations** (8 influential · 3.6/mo) · Qiuchen Wang, Ruixue Ding, Zehui Chen, Weiqi Wu et al.

## Abstract
Understanding information from visually rich documents remains a significant challenge for traditional Retrieval-Augmented Generation (RAG) methods. Existing benchmarks predominantly focus on image-based question answering (QA), overlooking the fundamental challenges of efficient retrieval, comprehension, and reasoning within dense visual documents. To bridge this gap, we introduce ViDoSeek, a novel dataset designed to evaluate RAG performance on visually rich documents requiring complex reasoning. Based on it, we identify key limitations in current RAG approaches: (i) purely visual retrieval methods struggle to effectively integrate both textual and visual features, and (ii) previous approaches often allocate insufficient reasoning tokens, limiting their effectiveness. To address these challenges, we propose ViDoRAG, a novel multi-agent RAG framework tailored for complex reasoning across visual documents. ViDoRAG employs a Gaussian Mixture Model (GMM)-based hybrid strategy to effectively handle multi-modal retrieval. To further elicit the model's reasoning capabilities, we introduce an iterative agent workflow incorporating exploration, summarization, and reflection, providing a framework for investigating test-time scaling in RAG domains. Extensive experiments on ViDoSeek validate the effectiveness and generalization of our approach. Notably, ViDoRAG outperforms existing methods by over 10% on the competitive ViDoSeek benchmark. The code is available at https://github.com/Alibaba-NLP/ViDoRAG.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Visual Document Q A Benchmarks. Retrieval-augmented Generation. 3 Problem Formulation 4 ViDoSeek Dataset 4.1 Dataset Construction. Step 1. Document Collecting. Step 2. Query Creation. Step 3. Quality Review. Step 4. Multimodal Refine. 4.2 Dataset Analysis Dataset Statistics. Comparative Analysis. 5 Method 5.1 Multi-Modal Hybrid Retrieval Adaptive Recall with Gaussian Mixture Model. Textual and Visual Hybrid Retrieval. 5.2 Multi-Agent Generation with Iterative Reasoning Seeker Agent: Hunting for relevant images. Inspector Agent: Review in detail and Reflect. Answer Agent: Synthesize the final answer. 6 Experiments 6.1 Experimental Settings Evaluation Metric Baselines and Oracle. 6.2 Main Results 6.3 Retrieval Evaluation 7 Analysis 7.1 Ablations 7.2 Time Efficiency How does dynamic retrieval balance latency and accuracy? Latency Analysis of the Multi-Agent Generation. 7.3 Modalities and Strategies of Generation 7.4 Performance with Test-time Scaling 8 Conc…

**Method / approach.** Method 5.1 Multi-Modal Hybrid Retrieval Adaptive Recall with Gaussian Mixture Model. Textual and Visual Hybrid Retrieval. 5.2 Multi-Agent Generation with Iterative Reasoning Seeker Agent: Hunting for relevant images. Inspector Agent: Review in detail and Reflect. Answer Agent: Synthesize the final answer. 6 Experiments 6.1 Experimental Settings Evaluation Metric Baselines and Oracle. 6.2 Main Results 6.3 Retrieval Evaluation 7 Analysis 7.1 Ablations 7.2 Time Efficiency How does dynamic retrieval balance latency and accuracy? Latency Analysis of the Multi-Agent Generation. 7.3 Modalities and Strategies of Generation 7.4 Performance with Test-time Scaling 8 Conclusion A Additional Experiments Details Backbones. Experimental Environments. Retrieval Implementation Details. B More Details on Datasets B.1 Annotation Case B.2 Details on ViDoSeek More Dataset Statistics. Dataset Difficulty. B.3 Detai…

**Results.** Experiments 6.1 Experimental Settings Evaluation Metric Baselines and Oracle. 6.2 Main Results 6.3 Retrieval Evaluation 7 Analysis 7.1 Ablations 7.2 Time Efficiency How does dynamic retrieval balance latency and accuracy? Latency Analysis of the Multi-Agent Generation. 7.3 Modalities and Strategies of Generation 7.4 Performance with Test-time Scaling 8 Conclusion A Additional Experiments Details Backbones. Experimental Environments. Retrieval Implementation Details. B More Details on Datasets B.1 Annotation Case B.2 Details on ViDoSeek More Dataset Statistics. Dataset Difficulty. B.3 Details on SlideVQA-Refined Dataset Statistics. Dataset Difficulty. C Data Construction Details Step 1. Document Collecting. Step 2. Query Creation. Step 3. Quality Review. Step 4. Multimodal Refine. D More Details about Multi-Agent Generation with Iterative Reasoni…

**Conclusion.** Conclusion A Additional Experiments Details Backbones. Experimental Environments. Retrieval Implementation Details. B More Details on Datasets B.1 Annotation Case B.2 Details on ViDoSeek More Dataset Statistics. Dataset Difficulty. B.3 Details on SlideVQA-Refined Dataset Statistics. Dataset Difficulty. C Data Construction Details Step 1. Document Collecting. Step 2. Query Creation. Step 3. Quality Review. Step 4. Multimodal Refine. D More Details about Multi-Agent Generation with Iterative Reasoning ViDoRAG: Visual Document Retrieval-Augmented Generation via Dynamic Iterative Reasoning Agents Qiuchen Wang 1 , Ruixue Ding 2 , Zehui Chen 1 , Weiqi Wu 3 , Shihang Wang 2 , Pengjun Xi…

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2502.18017v2.md` · `raw/arxiv/2502.18017v2.fulltext.md`
