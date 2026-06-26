---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A Survey of LLM-based Deep Search Agents: Paradigm, Optimization, Evaluation, and Challenges"
authors: Yunjia Xi, Jianghao Lin, Yongzhao Xiao, Zheli Zhou et al.
url: https://arxiv.org/abs/2508.05668v3
date: 2025-08-03
citationCount: 44
influentialCitationCount: 1
velocity: 4.15
ingested: 2026-06-22
tags: [coding-agents, agentic-ai, arxiv, 2025, cited]
---

# A Survey of LLM-based Deep Search Agents: Paradigm, Optimization, Evaluation, and Challenges

**arXiv [2508.05668v3](https://arxiv.org/abs/2508.05668v3)** · 2025-08-03 · **44 citations** (1 influential · 4.15/mo) · Yunjia Xi, Jianghao Lin, Yongzhao Xiao, Zheli Zhou et al.

## Abstract
The advent of Large Language Models (LLMs) has significantly revolutionized web search. The emergence of LLM-based Search Agents marks a pivotal shift towards deeper, dynamic, autonomous information seeking. These agents can comprehend user intentions and environmental context and execute multi-turn retrieval with dynamic planning, extending search capabilities far beyond the web. Leading examples like OpenAI's Deep Research highlight their potential for deep information mining and real-world applications. This survey provides the first systematic analysis of search agents. We comprehensively analyze and categorize existing works from the perspectives of architecture, optimization, application, and evaluation, ultimately identifying critical open challenges and outlining promising future research directions in this rapidly evolving field. Our repository is available on https://github.com/YunjiaXi/Awesome-Search-Agent-Papers.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Task Formulation 3 How to Search 3.1 Parallel Structure Decomposition-based Parallel Search. Diversification-based Parallel Search. 3.2 Sequential Structure Reflection-Driven Sequential Search. Proactivity-Driven Sequential Search. 3.3 Hybrid Structure Tree-based Search Graph-based Search 4 How to Optimize 4.1 Tuning-Free Approaches Single-Agent Architectures. Multi-Agent Architectures. Test-Time Scaling. 4.2 Tuning-based Approaches Supervised Fine-Tuning (SFT). Reinforcement Learning (RL). Mixed Approaches. 5 How to Apply 5.1 External Applications 5.2 Internal Applications Tool Use. Memory. Reasoning. 6 How to Evaluate 6.1 Datasets for Evaluation Closed-ended QA. Open-ended QA Dataset. Domain-Specific Dataset. 6.2 Metrics Judgment Metrics. Judge. 7 Challenges and Future Directions Broaden and Fuse Information Sources. Imperfect Retrieval. From Text to Multi-Modality. Customized Reinforcement Learning. Robust Infrastructure. Search Agent Self-Evolution.…

**Method / approach.** methodologies for search agents, including tuning and non-tuning approaches. How to Apply in Sec. 5 delineates the extensive application areas of search agents, encompassing both internal agent enhancements ( e.g. , reasoning, memory, and tool-use) and external applications ( e.g. , math, medicine, and finance). How to Evaluate in Sec. 5 introduces evaluation of search agents, covering various datasets and metrics. Finally, Sec. 7 presents current challenges and promising future research directions. Figure 2: Structural overview of Search Agent – how to search, how to optimize, how to apply, and how to evaluate. 2 Task Formulation Given a user’s intention q q and context C C , a search agent iteratively plans and acts to gather information and fulfill the user’s intention. Upon receiving intention q q , the agent initiates a planning π 0 = Plan ​ ( q , C ) \pi_{0}=\text{Plan}(q,C) to conduct an information seeking trajectory. At each step t t , the agent reflects on it…

**Results.** Evaluation, and Challenges 1 Introduction 2 Task Formulation 3 How to Search 3.1 Parallel Structure Decomposition-based Parallel Search. Diversification-based Parallel Search. 3.2 Sequential Structure Reflection-Driven Sequential Search. Proactivity-Driven Sequential Search. 3.3 Hybrid Structure Tree-based Search Graph-based Search 4 How to Optimize 4.1 Tuning-Free Approaches Single-Agent Architectures. Multi-Agent Architectures. Test-Time Scaling. 4.2 Tuning-based Approaches Supervised Fine-Tuning (SFT). Reinforcement Learning (RL). Mixed Approaches. 5 How to Apply 5.1 External Applications 5.2 Internal Applications Tool Use. Memory. Reasoning. 6 How to Evaluate 6.1 Datasets for Evaluation Closed-ended QA. Open-ended QA Dataset. Domain-Specific Dataset. 6.2 Metrics Judgment Metrics. Judge. 7 Challenges and Future Directions Bro…

**Conclusion.** Conclusion A Classification of Closed-ended QA Multi-hop QA Dataset. Challenging QA Dataset. Fact-Checking Dataset. B Detailed Challenges and Future Directions Broaden and Fuse Information Sources. Imperfect Retrieval. From Text to Multi-Modality. Customized Reinforcement Learning. Robust Infrastructure. Search Agent Self-Evolution. C Detailed Tables A Survey of LLM-based Deep Search Agents: Paradigm, Optimization, Evaluation, and Challenges Yunjia Xi 1 , Jianghao Lin 1 , Yongzhao Xiao 1 , Zheli Zhou 1 , Rong Shan 1 , Te Gao 2 , Jiachen Zhu 1 , Weiwen Liu 1 , Yong Yu 1 , Weinan Zhang 1 1 Shanghai Jiao Tong University, 2 Central South University {xiyunjia,linjianghao,wnzhang}@sjtu.edu.cn…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2508.05668v3.md` · `raw/arxiv/2508.05668v3.fulltext.md`
