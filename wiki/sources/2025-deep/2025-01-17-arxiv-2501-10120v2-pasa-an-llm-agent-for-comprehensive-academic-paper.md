---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PaSa: An LLM Agent for Comprehensive Academic Paper Search"
authors: Yichen He, Guanhua Huang, Peiyuan Feng, Yuan Lin et al.
url: https://arxiv.org/abs/2501.10120v2
date: 2025-01-17
citationCount: 64
influentialCitationCount: 8
velocity: 3.74
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# PaSa: An LLM Agent for Comprehensive Academic Paper Search

**arXiv [2501.10120v2](https://arxiv.org/abs/2501.10120v2)** · 2025-01-17 · **64 citations** (8 influential · 3.74/mo) · Yichen He, Guanhua Huang, Peiyuan Feng, Yuan Lin et al.

## Abstract
We introduce PaSa, an advanced Paper Search agent powered by large language models. PaSa can autonomously make a series of decisions, including invoking search tools, reading papers, and selecting relevant references, to ultimately obtain comprehensive and accurate results for complex scholar queries. We optimize PaSa using reinforcement learning with a synthetic dataset, AutoScholarQuery, which includes 35k fine-grained academic queries and corresponding papers sourced from top-tier AI conference publications. Additionally, we develop RealScholarQuery, a benchmark collecting real-world academic queries to assess PaSa performance in more realistic scenarios. Despite being trained on synthetic data, PaSa significantly outperforms existing baselines on RealScholarQuery, including Google, Google Scholar, Google with GPT-4o for paraphrased queries, ChatGPT (search-enabled GPT-4o), GPT-o1, and PaSa-GPT-4o (PaSa implemented by prompting GPT-4o). Notably, PaSa-7B surpasses the best Google-based baseline, Google with GPT-4o, by 37.78% in recall@20 and 39.90% in recall@50, and exceeds PaSa-GPT-4o by 30.36% in recall and 4.25% in precision. Model, datasets, and code are available at https://github.com/bytedance/pasa.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work LLMs in Scientific Discovery LLM Agents 3 Datasets 3.1 AutoScholarQuery 3.2 RealScholarQuery 4 Methodology 4.1 Overview 4.2 Crawler Reward Design RL Training 4.3 Selector 5 Experiments 5.1 Experimental Setting Selector Crawler Implementation of [Search] Paper Management 5.2 Baselines and Evaluation 5.3 Main results 5.4 Ablation study 6 Conclusion A Quality Evaluation of AutoScholarQuery B Annotation details B.1 Annotation Instructions B.2 Quality control C Example in RealScholarQuery D Implementation Details of the Crawler D.1 Imitation learning data generation D.2 PPO training E Implementation Details of the Selector F Selector Test Dataset G Additional Experimental Results G.1 Results on 100-sample subset of AutoScholarQuery G.2 Action cost H Prompt Templates H.1 Prompts used for data synthesis in AutoScholarQuery H.2 Prompts for baselines PaSa: An LLM Agent for Comprehensive Academic Paper Search Yichen He ∗ 1 Guanhua Huang ∗ 1 Pei…

**Method / approach.** Methodology 4.1 Overview 4.2 Crawler Reward Design RL Training 4.3 Selector 5 Experiments 5.1 Experimental Setting Selector Crawler Implementation of [Search] Paper Management 5.2 Baselines and Evaluation 5.3 Main results 5.4 Ablation study 6 Conclusion A Quality Evaluation of AutoScholarQuery B Annotation details B.1 Annotation Instructions B.2 Quality control C Example in RealScholarQuery D Implementation Details of the Crawler D.1 Imitation learning data generation D.2 PPO training E Implementation Details of the Selector F Selector Test Dataset G Additional Experimental Results G.1 Results on 100-sample subset of AutoScholarQuery G.2 Action cost H Prompt Templates H.1 Prompts used for data synthesis in AutoScholarQuery H.2 Prompts for baselines PaSa: An LLM Agent for Comprehensive Academic Paper Search Yichen He ∗ 1 Guanhua Huang ∗ 1 Peiyuan Feng 1 Yuan Lin † 1 Yuchen Zhang…

**Results.** Experiments 5.1 Experimental Setting Selector Crawler Implementation of [Search] Paper Management 5.2 Baselines and Evaluation 5.3 Main results 5.4 Ablation study 6 Conclusion A Quality Evaluation of AutoScholarQuery B Annotation details B.1 Annotation Instructions B.2 Quality control C Example in RealScholarQuery D Implementation Details of the Crawler D.1 Imitation learning data generation D.2 PPO training E Implementation Details of the Selector F Selector Test Dataset G Additional Experimental Results G.1 Results on 100-sample subset of AutoScholarQuery G.2 Action cost H Prompt Templates H.1 Prompts used for data synthesis in AutoScholarQuery H.2 Prompts for baselines PaSa: An LLM Agent for Comprehensive Academic Paper Search Yichen He ∗ 1 Guanhua Huang ∗ 1 Peiyuan Feng 1 Yuan Lin † 1 Yuchen Zhang 1 Hang Li 1 Weinan E 2 1 ByteDance Seed…

**Conclusion.** Conclusion A Quality Evaluation of AutoScholarQuery B Annotation details B.1 Annotation Instructions B.2 Quality control C Example in RealScholarQuery D Implementation Details of the Crawler D.1 Imitation learning data generation D.2 PPO training E Implementation Details of the Selector F Selector Test Dataset G Additional Experimental Results G.1 Results on 100-sample subset of AutoScholarQuery G.2 Action cost H Prompt Templates H.1 Prompts used for data synthesis in AutoScholarQuery H.2 Prompts for baselines PaSa: An LLM Agent for Comprehensive Academic Paper Search Yichen He ∗ 1 Guanhua Huang ∗ 1 Peiyuan Feng 1 Yuan Lin † 1 Yuchen Zhang 1 Hang Li 1 Weinan E 2 1 Byte…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2501.10120v2.md` · `raw/arxiv/2501.10120v2.fulltext.md`
