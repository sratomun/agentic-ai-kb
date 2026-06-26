---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment"
authors: Xiangjin Xie, Guangwei Xu, Lingyan Zhao, Ruijie Guo
url: https://arxiv.org/abs/2502.14913v1
date: 2025-02-19
citationCount: 76
influentialCitationCount: 15
velocity: 4.74
ingested: 2026-06-22
tags: [data-query-agents, agent-reliability, agentic-rl, multi-agent-systems, agentic-ai, arxiv, 2025, cited]
---

# OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment

**arXiv [2502.14913v1](https://arxiv.org/abs/2502.14913v1)** · 2025-02-19 · **76 citations** (15 influential · 4.74/mo) · Xiangjin Xie, Guangwei Xu, Lingyan Zhao, Ruijie Guo

## Abstract
Although multi-agent collaborative Large Language Models (LLMs) have achieved significant breakthroughs in the Text-to-SQL task, their performance is still constrained by various factors. These factors include the incompleteness of the framework, failure to follow instructions, and model hallucination problems. To address these problems, we propose OpenSearch-SQL, which divides the Text-to-SQL task into four main modules: Preprocessing, Extraction, Generation, and Refinement, along with an Alignment module based on a consistency alignment mechanism. This architecture aligns the inputs and outputs of agents through the Alignment module, reducing failures in instruction following and hallucination. Additionally, we designed an intermediate language called SQL-Like and optimized the structured CoT based on SQL-Like. Meanwhile, we developed a dynamic few-shot strategy in the form of self-taught Query-CoT-SQL. These methods have significantly improved the performance of LLMs in the Text-to-SQL task. In terms of model selection, we directly applied the base LLMs without any post-training, thereby simplifying the task chain and enhancing the framework's portability. Experimental results show that OpenSearch-SQL achieves an execution accuracy(EX) of 69.3% on the BIRD development set, 72.28% on the test set, and a reward-based validity efficiency score (R-VES) of 69.36%, with all three metrics ranking first at the time of submission. These results demonstrate the comprehensive advantages of the proposed method in both effectiveness and efficiency.

## From the paper (full-text excerpts)
**Introduction.** Introduction Framework. 2 Preliminary 2.1 Large Language Models 2.2 Text-to-SQL 2.3 Hallucination 3 Methodology 3.1 Alignments 3.2 Self-Taught Fewshot 3.3 Preprocessing 3.4 Extraction Entity Extraction Values Retrieval. Column Filtering. Info Alignment 3.5 Generation SQL Generation. Alignments 3.6 Refinement 3.7 Algorithm 3.8 Optimization 4 Experiments 4.1 Experimental Setup Datasets BIRD Spider Evaluation Baselines Implementation Details 4.2 Main Result BIRD Results Spider Results 4.3 Modular Ablation 4.4 Few-shot 4.5 Self-Consistency Vote 4.6 Execution Cost 4.7 CoT 5 Conclusion OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment Xiangjin Xie xiexiangjin.xxj@alibaba-inc.com Alibaba Cloud China , Guangwei Xu kunka.xgw@alibaba-inc.com Alibaba Cloud China , LingYan Zhao zhaolingyan.zly@alibaba-inc.com Alibaba Cloud China and Ruijie Guo ruijie.guo@alibaba-inc.com Alibaba Cloud China (2018; 20 Febru…

**Method / approach.** Methodology 3.1 Alignments 3.2 Self-Taught Fewshot 3.3 Preprocessing 3.4 Extraction Entity Extraction Values Retrieval. Column Filtering. Info Alignment 3.5 Generation SQL Generation. Alignments 3.6 Refinement 3.7 Algorithm 3.8 Optimization 4 Experiments 4.1 Experimental Setup Datasets BIRD Spider Evaluation Baselines Implementation Details 4.2 Main Result BIRD Results Spider Results 4.3 Modular Ablation 4.4 Few-shot 4.5 Self-Consistency Vote 4.6 Execution Cost 4.7 CoT 5 Conclusion OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment Xiangjin Xie xiexiangjin.xxj@alibaba-inc.com Alibaba Cloud China , Guangwei Xu kunka.xgw@alibaba-inc.com Alibaba Cloud China , LingYan Zhao zhaolingyan.zly@alibaba-inc.com Alibaba Cloud China and Ruijie Guo ruijie.guo@alibaba-inc.com Alibaba Cloud China (2018; 20 February 2007; 12 Marc…

**Results.** Experiments 4.1 Experimental Setup Datasets BIRD Spider Evaluation Baselines Implementation Details 4.2 Main Result BIRD Results Spider Results 4.3 Modular Ablation 4.4 Few-shot 4.5 Self-Consistency Vote 4.6 Execution Cost 4.7 CoT 5 Conclusion OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment Xiangjin Xie xiexiangjin.xxj@alibaba-inc.com Alibaba Cloud China , Guangwei Xu kunka.xgw@alibaba-inc.com Alibaba Cloud China , LingYan Zhao zhaolingyan.zly@alibaba-inc.com Alibaba Cloud China and Ruijie Guo ruijie.guo@alibaba-inc.com Alibaba Cloud China (2018; 20 February 2007; 12 March 2009; 5 June 2009) Abstract. Although multi-agent collaborative Large Language Models (LLMs) have achieved significant breakthroughs in the Text-to-SQL task, their performance is still constrained by various factors. These fact…

**Conclusion.** Conclusion OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Alignment Xiangjin Xie xiexiangjin.xxj@alibaba-inc.com Alibaba Cloud China , Guangwei Xu kunka.xgw@alibaba-inc.com Alibaba Cloud China , LingYan Zhao zhaolingyan.zly@alibaba-inc.com Alibaba Cloud China and Ruijie Guo ruijie.guo@alibaba-inc.com Alibaba Cloud China (2018; 20 February 2007; 12 March 2009; 5 June 2009) Abstract. Although multi-agent collaborative Large Language Models (LLMs) have achieved significant breakthroughs in the Text-to-SQL task, their performance is still constrained by various factors. These factors include the incompleteness of the framework, failure to follow instru…

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[bird-benchmark]]
- **Raw:** `raw/arxiv/2502.14913v1.md` · `raw/arxiv/2502.14913v1.fulltext.md`
