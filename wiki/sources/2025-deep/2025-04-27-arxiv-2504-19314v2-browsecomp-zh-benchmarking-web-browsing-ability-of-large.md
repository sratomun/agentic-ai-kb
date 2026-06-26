---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "BrowseComp-ZH: Benchmarking Web Browsing Ability of Large Language Models in Chinese"
authors: Peilin Zhou, Bruce Leon, Xiang Ying, Can Zhang et al.
url: https://arxiv.org/abs/2504.19314v2
date: 2025-04-27
citationCount: 104
influentialCitationCount: 23
velocity: 7.52
ingested: 2026-06-22
tags: [computer-use-agents, agent-protocols, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# BrowseComp-ZH: Benchmarking Web Browsing Ability of Large Language Models in Chinese

**arXiv [2504.19314v2](https://arxiv.org/abs/2504.19314v2)** · 2025-04-27 · **104 citations** (23 influential · 7.52/mo) · Peilin Zhou, Bruce Leon, Xiang Ying, Can Zhang et al.

## Abstract
As large language models (LLMs) evolve into tool-using agents, the ability to browse the web in real-time has become a critical yardstick for measuring their reasoning and retrieval competence. Existing benchmarks such as BrowseComp concentrate on English and overlook the linguistic, infrastructural, and censorship-related complexities of other major information ecosystems -- most notably Chinese. To address this gap, we introduce BrowseComp-ZH, a high-difficulty benchmark purpose-built to comprehensively evaluate LLM agents on the Chinese web. BrowseComp-ZH consists of 289 multi-hop questions spanning 11 diverse domains. Each question is reverse-engineered from a short, objective, and easily verifiable answer (e.g., a date, number, or proper noun). A two-stage quality control protocol is applied to strive for high question difficulty and answer uniqueness. We benchmark over 20 state-of-the-art language models and agentic search systems on our proposed BrowseComp-ZH. Despite their strong conversational and retrieval capabilities, most models struggle severely: a large number achieve accuracy rates below 10%, and only a handful exceed 20%. Even the best-performing system, OpenAI's DeepResearch, reaches just 42.9%. These results demonstrate the considerable difficulty of BrowseComp-ZH, where success demands not only effective retrieval strategies, but also sophisticated reasoning and information reconciliation -- capabilities that current models still struggle to master. Our dataset, construction guidelines, and benchmark results have been publicly released at https://github.com/PALIN2018/BrowseComp-ZH.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 The BrowseComp-ZH Dataset 3.1 Dataset Construction Stage 1: Topic and Answer Selection Stage 2: Reverse Question Design 3.2 Quality Control Stage 1: Question Difficulty Validation Stage 2: Answer Uniqueness Validation 3.3 Data Statistics 4 Benchmarks 4.1 Models 4.2 Setting 4.3 Metrics 4.4 Performance 4.5 Analysis of Reasoning Ability of LLM 4.6 Analysis of AI Search Products 4.7 Calibration Analysis 5 Conclusion and Discussion Future Work A Technical Appendices and Supplementary Material A.1 Instructions for model prediction A.2 Instruction for grading BrowseComp-ZH: Benchmarking Web Browsing Ability of Large Language Models in Chinese Peilin Zhou 1† Bruce Leon 2† Xiang Ying 3 Can Zhang 2 Yifan Shao Qichen Ye 4 Dading Chong 2 Zhiling Jin 5 Chenxuan Xie 6 Meng Cao 7 Yuxin Gu 8 Sixin Hong 2 Jing Ren 2 Jian Chen 1,9 Chao Liu 2 Yining Hua 10 1 Hong Kong University of Science and Technology (Guangzhou) 2 Peking University 3 Mindverse AI 4 Alibaba Group 5 Zhe…

**Method / approach.** methods including introducing implicit constraints or obfuscating key lexical signals. This process yields 480 preliminary samples, which are subsequently reviewed via the quality control procedure detailed in Section 3.2 . 3.2 Quality Control To ensure the rigor and challenge of BrowseComp-ZH, we implement a two-stage quality control protocol: one focusing on question difficulty and the other on answer uniqueness. Stage 1: Question Difficulty Validation Although annotators are required to check whether a question can be quickly solved by search engines during the design process, variations in search ability and prior knowledge could introduce inconsistencies, leading to the inclusion of overly simple questions. To address this, we conduct a cross-checking phase: • Each annotator validates questions written by others using only search engines (no LLMs); • A strict 10-minute time limit is applied per question; • If the answer is found within the time…

**Results.** evaluation of browsing capabilities themselves—i.e., the ability of LLMs to effectively retrieve, filter, and reason over information from the web. This evaluation is crucial for assessing the true web-browsing competence of LLMs and understanding their potential to tackle real-world tasks that require dynamic information retrieval. To address this gap, Wei et al . ( 2025 ) introduced a benchmark of reverse-designed, evidence-grounded queries that challenge English-language agents to search and reason over difficult-to-access information. Nonetheless, Wei et al . ( 2025 ) primarily operates within the English-language web, missing the linguistic, structural, and cultural complexities inherent to other language environments. In particular, the Chinese web poses unique challenges for retrieval and reasoning: information is scattered across heterogeneous platforms (e.g., Baidu Baike, Zhihu, government portals), naming conventions are in…

**Conclusion.** Conclusion and Discussion Future Work A Technical Appendices and Supplementary Material A.1 Instructions for model prediction A.2 Instruction for grading BrowseComp-ZH: Benchmarking Web Browsing Ability of Large Language Models in Chinese Peilin Zhou 1† Bruce Leon 2† Xiang Ying 3 Can Zhang 2 Yifan Shao Qichen Ye 4 Dading Chong 2 Zhiling Jin 5 Chenxuan Xie 6 Meng Cao 7 Yuxin Gu 8 Sixin Hong 2 Jing Ren 2 Jian Chen 1,9 Chao Liu 2 Yining Hua 10 1 Hong Kong University of Science and Technology (Guangzhou) 2 Peking University 3 Mindverse AI 4 Alibaba Group 5 Zhejiang University 6 Zhejiang University of Technology 7 MBZUAI 8 NIO 9 HSBC 10 Harvard T.H. Chan School of Public Health {z…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[browsecomp]]
- **Raw:** `raw/arxiv/2504.19314v2.md` · `raw/arxiv/2504.19314v2.fulltext.md`
