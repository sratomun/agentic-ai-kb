---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "BrowseComp-Plus: A More Fair and Transparent Evaluation Benchmark of Deep-Research Agent"
authors: Zijian Chen, Xueguang Ma, Shengyao Zhuang, Ping Nie et al.
url: https://arxiv.org/abs/2508.06600v1
date: 2025-08-08
citationCount: 118
influentialCitationCount: 28
velocity: 11.3
ingested: 2026-06-22
tags: [science-agents, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# BrowseComp-Plus: A More Fair and Transparent Evaluation Benchmark of Deep-Research Agent

**arXiv [2508.06600v1](https://arxiv.org/abs/2508.06600v1)** · 2025-08-08 · **118 citations** (28 influential · 11.3/mo) · Zijian Chen, Xueguang Ma, Shengyao Zhuang, Ping Nie et al.

## Abstract
Deep-Research agents, which integrate large language models (LLMs) with search tools, have shown success in improving the effectiveness of handling complex queries that require iterative search planning and reasoning over search results. Evaluations on current benchmarks like BrowseComp relies on black-box live web search APIs, have notable limitations in (1) fairness: dynamic and opaque web APIs hinder fair comparisons and reproducibility of deep research methods; (2) transparency: lack of control over the document corpus makes it difficult to isolate retriever contributions. In other words, the current evaluations may compare a complete deep research system at a given time, but they do not foster well-controlled experiments to provide insights into the capability of underlying deep research LLMs. To address these challenges, we introduce BrowseComp-Plus, a benchmark derived from BrowseComp, employing a fixed, carefully curated corpus. Each query in BrowseComp-Plus includes human-verified supporting documents and mined challenging negatives, enabling controlled experimentation. The benchmark is shown to be effective in distinguishing the performance of deep research systems. For instance, the open-source model Search-R1, when paired with the BM25 retriever, achieves 3.86% accuracy, whereas the GPT-5 achieves 55.9%. Integrating the GPT-5 with the Qwen3-Embedding-8B retriever further enhances its accuracy to 70.1% with fewer search calls. This benchmark allows comprehensive evaluation and disentangled analysis of deep research agents and retrieval methods, fostering insights into retrieval effectiveness, citation accuracy, and context engineering in Deep-Research system.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works 2.1 Deep-Research Agent 2.2 Neural Retrieval 2.3 Deep Retrieval Benchmarks 3 BrowseComp-Plus 3.1 Preliminary: BrowseComp 3.2 Building the Document Corpus 3.2.1 Evidence Document Gathering 3.2.2 Evidence Document Verification 3.3 Hard Negative Mining 3.4 Final Corpus Statistics 4 Experiments 4.1 Baselines: LLM Search Agents 4.2 Baselines: Retriever 4.3 Experiment Setup Search Agents Retriever 4.4 Evaluation Metrics Deep Research Effectiveness Retrieval Effectiveness 4.5 Results 4.6 End-to-End Deep-Research Performance 4.7 Effect of Retrieval Quality 4.8 Analysis and Ablation 4.8.1 Oracle Retrieval 4.8.2 Impact of Reasoning Effort 4.8.3 Effect of Document Reading Strategy 4.8.4 Effect of Corpus Size 5 Future Work and Discussion 6 Conclusion A OpenAI O3 Evidence Document Gathering Prompt B Labelling UI Example C Problematic Cases D Negative Mining Query Decomposition Prompt E Main Search Prompt F Evaluation Prompt G Search Prompt with Get-Doc H API Cost…

**Method / approach.** methods; (2) transparency : lack of control over the document corpus makes it difficult to isolate retriever contributions. In other words, the current evaluations may compare a complete deep research system at a given time, but they do not foster well-controlled experiments to provide insights into the capability of underlying deep research LLMs. To address these challenges, we introduce BrowseComp-Plus , a benchmark derived from BrowseComp, employing a fixed, carefully curated corpus. Each query in BrowseComp-Plus includes human-verified supporting documents and mined challenging negatives, enabling controlled experimentation. The benchmark is shown to be effective in distinguishing the performance of deep research systems. For instance, the open-source model Search-R1, when paired with the BM25 retriever, achieves 3.86% accuracy, whereas the GPT-5 achieves 55.9%. Integrating the GPT-5 with the Qwen3-Embedding-8B retriever further enhances its accuracy to 70.1% with fewer search cal…

**Results.** Experiments 4.1 Baselines: LLM Search Agents 4.2 Baselines: Retriever 4.3 Experiment Setup Search Agents Retriever 4.4 Evaluation Metrics Deep Research Effectiveness Retrieval Effectiveness 4.5 Results 4.6 End-to-End Deep-Research Performance 4.7 Effect of Retrieval Quality 4.8 Analysis and Ablation 4.8.1 Oracle Retrieval 4.8.2 Impact of Reasoning Effort 4.8.3 Effect of Document Reading Strategy 4.8.4 Effect of Corpus Size 5 Future Work and Discussion 6 Conclusion A OpenAI O3 Evidence Document Gathering Prompt B Labelling UI Example C Problematic Cases D Negative Mining Query Decomposition Prompt E Main Search Prompt F Evaluation Prompt G Search Prompt with Get-Doc H API Cost BrowseComp-Plus: A More Fair and Transparent Evaluation Benchmark of Deep-Research Agent Zijian Chen , ​ 1 {}^{\text{,}1} , Xueguang Ma ∗ , \faEnvelopeO {}^{*\text{,~\faEnvelopeO}} , ​ 1 {}^…

**Conclusion.** Conclusion A OpenAI O3 Evidence Document Gathering Prompt B Labelling UI Example C Problematic Cases D Negative Mining Query Decomposition Prompt E Main Search Prompt F Evaluation Prompt G Search Prompt with Get-Doc H API Cost BrowseComp-Plus: A More Fair and Transparent Evaluation Benchmark of Deep-Research Agent Zijian Chen , ​ 1 {}^{\text{,}1} , Xueguang Ma ∗ , \faEnvelopeO {}^{*\text{,~\faEnvelopeO}} , ​ 1 {}^{\text{,}1} , Shengyao Zhuang ∗ , ​ 2 ​ , ​ 5 {}^{\text{,}2\text{,}5} , Ping Nie 3 , Kai Zou 3 , Andrew Liu 1 , Joshua Green 1 , Kshama Patel 1 , Ruoxi Meng 1 , Mingyi Su 1 , Sahel Sharifymoghaddam 1 , Yanxi Li 1 , Haoran Hong 1 , Xinyu Shi 1 , Xuye Liu 1 , Nandan Thakur 1 , Crystina Zhang 1 , Luyu Gao…

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[qwen]] · [[gpt-5]] · [[browsecomp]]
- **Raw:** `raw/arxiv/2508.06600v1.md` · `raw/arxiv/2508.06600v1.fulltext.md`
