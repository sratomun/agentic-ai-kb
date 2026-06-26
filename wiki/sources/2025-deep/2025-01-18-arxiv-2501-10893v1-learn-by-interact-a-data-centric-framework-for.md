---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments"
authors: Hongjin Su, Ruoxi Sun, Jinsung Yoon, Pengcheng Yin et al.
url: https://arxiv.org/abs/2501.10893v1
date: 2025-01-18
citationCount: 80
influentialCitationCount: 7
velocity: 4.68
ingested: 2026-06-22
tags: [coding-agents, agentic-rag, agentic-ai, arxiv, 2025, cited]
---

# Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments

**arXiv [2501.10893v1](https://arxiv.org/abs/2501.10893v1)** · 2025-01-18 · **80 citations** (7 influential · 4.68/mo) · Hongjin Su, Ruoxi Sun, Jinsung Yoon, Pengcheng Yin et al.

## Abstract
Autonomous agents powered by large language models (LLMs) have the potential to enhance human capabilities, assisting with digital tasks from sending emails to performing data analysis. The abilities of existing LLMs at such tasks are often hindered by the lack of high-quality agent data from the corresponding environments they interact with. We propose Learn-by-interact, a data-centric framework to adapt LLM agents to any given environments without human annotations. Learn-by-interact synthesizes trajectories of agent-environment interactions based on documentations, and constructs instructions by summarizing or abstracting the interaction histories, a process called backward construction. We assess the quality of our synthetic data by using them in both training-based scenarios and training-free in-context learning (ICL), where we craft innovative retrieval approaches optimized for agents. Extensive experiments on SWE-bench, WebArena, OSWorld and Spider2-V spanning across realistic coding, web, and desktop environments show the effectiveness of Learn-by-interact in various downstream agentic tasks -- baseline results are improved by up to 12.2\% for ICL with Claude-3.5 and 19.5\% for training with Codestral-22B. We further demonstrate the critical role of backward construction, which provides up to 14.0\% improvement for training. Our ablation studies demonstrate the efficiency provided by our synthesized data in ICL and the superiority of our retrieval pipeline over alternative approaches like conventional retrieval-augmented generation (RAG). We expect that Learn-by-interact will serve as a foundation for agent data synthesis as LLMs are increasingly deployed at real-world environments.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Learn-by-interact 2.1 Task formulation 2.2 Agentic data synthesis 2.3 Filtering 2.4 Adaptation 3 Experiments 3.1 Baselines 3.2 Datasets 3.3 Settings 3.4 Evaluation 3.5 Results 3.5.1 Training-free Evaluation 3.5.2 Training-based Evaluation 4 Analysis 4.1 Inference Efficiency 4.2 The Impact of Retrieval 4.3 Data granularity 4.4 Scaling Laws 5 Related work 6 Conclusion 7 Limitations A Baseline implementations B Dataset examples C Experimental settings D Document sources E Synthesized data examples F Case study on filtered examples G Synthesized data from environments H Cross-website generalization \pdftrailerid redacted \correspondingauthor hjsu@cs.hku.hk Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments Hongjin Su Ruoxi Sun Google Jinsung Yoon Google Pengcheng Yin Google Tao Yu The University of Hong Kong Sercan Ö. Arık Google Abstract Autonomous agents powered by large language models (LLMs) have the potential to…

**Method / approach.** methods can be applied to the commercial LLMs even with prediction-only API access. Results on Table 2 show marginal improvement of RAG compared to the baseline, which suggests limited effectiveness by simply concatenating standard resources to LLM prompts. By retrieving examples from distilled data, we observe better performance compared to RAG, but still no more than 2% improvement over the baseline, which indicates that the distilled data tend to be noisy in the setting with multi-round agent-environment interactions. This highlights the critical role of backward construction, which corrects the misalignment between instructions and trajectories by curating new task objectives. Both Reflexion and LATS consistently improve over the baseline across 4 benchmarks, which demonstrate their general applicability to agent tasks. Using the data synthesized from the Learn-by-interact , we can see a significant performance gain compared to all other frameworks in both Gemini and Claude…

**Results.** Experiments 3.1 Baselines 3.2 Datasets 3.3 Settings 3.4 Evaluation 3.5 Results 3.5.1 Training-free Evaluation 3.5.2 Training-based Evaluation 4 Analysis 4.1 Inference Efficiency 4.2 The Impact of Retrieval 4.3 Data granularity 4.4 Scaling Laws 5 Related work 6 Conclusion 7 Limitations A Baseline implementations B Dataset examples C Experimental settings D Document sources E Synthesized data examples F Case study on filtered examples G Synthesized data from environments H Cross-website generalization \pdftrailerid redacted \correspondingauthor hjsu@cs.hku.hk Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments Hongjin Su Ruoxi Sun Google Jinsung Yoon Google Pengcheng Yin Google Tao Yu The University of Hong Kong Sercan Ö. Arık Google Abstract Autonomous agents powered by large language models (LLMs) h…

**Conclusion.** Conclusion 7 Limitations A Baseline implementations B Dataset examples C Experimental settings D Document sources E Synthesized data examples F Case study on filtered examples G Synthesized data from environments H Cross-website generalization \pdftrailerid redacted \correspondingauthor hjsu@cs.hku.hk Learn-by-interact: A Data-Centric Framework for Self-Adaptive Agents in Realistic Environments Hongjin Su Ruoxi Sun Google Jinsung Yoon Google Pengcheng Yin Google Tao Yu The University of Hong Kong Sercan Ö. Arık Google Abstract Autonomous agents powered by large language models (LLMs) have the potential to enhance human capabilities, assisting with digital tasks from sending emails t…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rag|Agentic RAG]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]] · [[osworld]] · [[webarena]] · [[claude]]
- **Raw:** `raw/arxiv/2501.10893v1.md` · `raw/arxiv/2501.10893v1.fulltext.md`
