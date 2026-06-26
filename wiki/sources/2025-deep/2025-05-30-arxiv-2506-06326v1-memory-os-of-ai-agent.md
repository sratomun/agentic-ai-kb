---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memory OS of AI Agent"
authors: Jiazheng Kang, Mingming Ji, Zhe Zhao, Ting Bai
url: https://arxiv.org/abs/2506.06326v1
date: 2025-05-30
citationCount: 74
influentialCitationCount: 14
velocity: 5.81
ingested: 2026-06-22
tags: [agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Memory OS of AI Agent

**arXiv [2506.06326v1](https://arxiv.org/abs/2506.06326v1)** · 2025-05-30 · **74 citations** (14 influential · 5.81/mo) · Jiazheng Kang, Mingming Ji, Zhe Zhao, Ting Bai

## Abstract
Large Language Models (LLMs) face a crucial challenge from fixed context windows and inadequate memory management, leading to a severe shortage of long-term memory capabilities and limited personalization in the interactive experience with AI agents. To overcome this challenge, we innovatively propose a Memory Operating System, i.e., MemoryOS, to achieve comprehensive and efficient memory management for AI agents. Inspired by the memory management principles in operating systems, MemoryOS designs a hierarchical storage architecture and consists of four key modules: Memory Storage, Updating, Retrieval, and Generation. Specifically, the architecture comprises three levels of storage units: short-term memory, mid-term memory, and long-term personal memory. Key operations within MemoryOS include dynamic updates between storage units: short-term to mid-term updates follow a dialogue-chain-based FIFO principle, while mid-term to long-term updates use a segmented page organization strategy. Our pioneering MemoryOS enables hierarchical memory integration and dynamic updating. Extensive experiments on the LoCoMo benchmark show an average improvement of 49.11% on F1 and 46.18% on BLEU-1 over the baselines on GPT-4o-mini, showing contextual coherence and personalized memory retention in long conversations. The implementation code is open-sourced at https://github.com/BAI-LAB/MemoryOS.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Memory for LLM Agents 2.2 Memory Management in OS 3 MemoryOS 3.1 Overview Architecture Memory Storage: Memory Updating: Memory Retrieval: Response Generation: 3.2 Memory Storage Module Short-Term Memory (STM): Mid-Term Memory (MTM): Long-term Persona Memory (LPM): 3.3 Memory Update Module STM-MTM Update: MTM-LPM Update: LPM Update: 3.4 Memory Retrieval Module STM retrieval: MTM retrieval: LPM retrieval: 3.5 Response Generation Module 4 Experiments 4.1 Experimental Settings Datasets. Evaluation Metrics. Compared Methods. TiM (Think-in-Memory) [ Liu et al.(2023)Liu, Yang, Shen, Hu, Zhang, Gu, and Zhang ] : MemoryBank [ Zhong et al.(2024)Zhong, Guo, Gao, Ye, and Wang ] : MemGPT [ Packer et al.(2023)Packer, Fang, Patil, Lin, Wooders, and Gonzalez ] : A-Mem (Agentic Memory) [ Xu et al.(2025)Xu, Liang, Mei, Gao, Tan, and Zhang ] : MemoryOS : Implementation Details. 4.2 Main Results 4.3 Ablation Study 4.4 Hyperparameter Analysis 4.5 Case Study 5 Conclusion…

**Method / approach.** Methods. TiM (Think-in-Memory) [ Liu et al.(2023)Liu, Yang, Shen, Hu, Zhang, Gu, and Zhang ] : MemoryBank [ Zhong et al.(2024)Zhong, Guo, Gao, Ye, and Wang ] : MemGPT [ Packer et al.(2023)Packer, Fang, Patil, Lin, Wooders, and Gonzalez ] : A-Mem (Agentic Memory) [ Xu et al.(2025)Xu, Liang, Mei, Gao, Tan, and Zhang ] : MemoryOS : Implementation Details. 4.2 Main Results 4.3 Ablation Study 4.4 Hyperparameter Analysis 4.5 Case Study 5 Conclusion Memory OS of AI Agent Jiazheng Kang Beijing University of Posts and Telecommunications kjz@bupt.edu.cn Mingming Ji Tencent AI Lab matthhewj@tencent.com \AND Zhe Zhao Tencent AI Lab nlpzhezhao@tencent.com Ting Bai Beijing University of Posts and Telecommunications baiting@bupt.edu.cn Corresponding author. Abstract Large Language Models (LLMs) face a crucial challenge from fixed context windows and inadequate memory management, leading to a severe shortage of long-term memory capabil…

**Results.** Experiments 4.1 Experimental Settings Datasets. Evaluation Metrics. Compared Methods. TiM (Think-in-Memory) [ Liu et al.(2023)Liu, Yang, Shen, Hu, Zhang, Gu, and Zhang ] : MemoryBank [ Zhong et al.(2024)Zhong, Guo, Gao, Ye, and Wang ] : MemGPT [ Packer et al.(2023)Packer, Fang, Patil, Lin, Wooders, and Gonzalez ] : A-Mem (Agentic Memory) [ Xu et al.(2025)Xu, Liang, Mei, Gao, Tan, and Zhang ] : MemoryOS : Implementation Details. 4.2 Main Results 4.3 Ablation Study 4.4 Hyperparameter Analysis 4.5 Case Study 5 Conclusion Memory OS of AI Agent Jiazheng Kang Beijing University of Posts and Telecommunications kjz@bupt.edu.cn Mingming Ji Tencent AI Lab matthhewj@tencent.com \AND Zhe Zhao Tencent AI Lab nlpzhezhao@tencent.com Ting Bai Beijing University of Posts and Telecommunications baiting@bupt.edu.cn Corresponding author. Abstract Large Language Models (LLMs) face…

**Conclusion.** Conclusion Memory OS of AI Agent Jiazheng Kang Beijing University of Posts and Telecommunications kjz@bupt.edu.cn Mingming Ji Tencent AI Lab matthhewj@tencent.com \AND Zhe Zhao Tencent AI Lab nlpzhezhao@tencent.com Ting Bai Beijing University of Posts and Telecommunications baiting@bupt.edu.cn Corresponding author. Abstract Large Language Models (LLMs) face a crucial challenge from fixed context windows and inadequate memory management, leading to a severe shortage of long-term memory capabilities and limited personalization in the interactive experience with AI agents. To overcome this challenge, we innovatively propose a Memory O perating S ystem, i.e., MemoryOS , to achieve comprehensive and efficien…

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2506.06326v1.md` · `raw/arxiv/2506.06326v1.fulltext.md`
