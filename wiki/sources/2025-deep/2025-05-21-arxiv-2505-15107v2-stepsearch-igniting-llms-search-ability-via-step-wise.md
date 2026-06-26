---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization"
authors: Ziliang Wang, Xuhui Zheng, Kang An, Cijun Ouyang et al.
url: https://arxiv.org/abs/2505.15107v2
date: 2025-05-21
citationCount: 54
influentialCitationCount: 12
velocity: 4.14
ingested: 2026-06-22
tags: [agentic-rl, agent-evaluation, arxiv, 2025, cited]
---

# StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization

**arXiv [2505.15107v2](https://arxiv.org/abs/2505.15107v2)** · 2025-05-21 · **54 citations** (12 influential · 4.14/mo) · Ziliang Wang, Xuhui Zheng, Kang An, Cijun Ouyang et al.

## Abstract
Efficient multi-hop reasoning requires Large Language Models (LLMs) based agents to acquire high-value external knowledge iteratively. Previous work has explored reinforcement learning (RL) to train LLMs to perform search-based document retrieval, achieving notable improvements in QA performance, but underperform on complex, multi-hop QA resulting from the sparse rewards from global signal only. To address this gap in existing research, we introduce StepSearch, a framework for search LLMs that trained with step-wise proximal policy optimization method. It consists of richer and more detailed intermediate search rewards and token-level process supervision based on information gain and redundancy penalties to better guide each search step. We constructed a fine-grained question-answering dataset containing sub-question-level search trajectories based on open source datasets through a set of data pipeline method. On standard multi-hop QA benchmarks, it significantly outperforms global-reward baselines, achieving 11.2% and 4.2% absolute improvements for 3B and 7B models over various search with RL baselines using only 19k training data, demonstrating the effectiveness of fine-grained, stepwise supervision in optimizing deep search LLMs. Our code will be released on https://github.com/Zillwang/StepSearch.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Methodology 2.1 Data Augmentation Pipeline 2.2 Train LLM with Search Actions 2.3 StepSearch 2.3.1 Type 1 Reward: Global Signal 2.3.2 Type 2 Reward: Search Step 3 Experiment 3.1 Dataset and Evaluation Metrics 3.2 Baselines 3.3 Training Details 3.4 Main Results 4 Further Analysis 4.1 Different RL Comparison 4.2 Ablation Study 4.3 Case Study 5 Limitations 6 Future Work A Prompt for Research Plan on Question Answering B Experiment Setups C Case Study StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization Ziliang Wang 1∗‡ , Xuhui Zheng 1,2 , Kang An 1,3∗† , Cijun Ouyang 1 , Jialu Cai 1 , Yuhang Wang 1 , Yichao Wu 1 1 SenseTime 2 Nanjing University 3 Shenzhen University {wangziliang1, ouyangcijun, caijialu, wangyuhang, wuyichao}@sensetime.com zhengxuhui@smail.nju.edu.cn, ankang@gml.ac.cn Equal contributionWork done during internship at SenseTime Project leader Corresponding author Abstract Efficient multi-hop reasoning requires Large Language Models (LLMs…

**Method / approach.** Methodology 2.1 Data Augmentation Pipeline 2.2 Train LLM with Search Actions 2.3 StepSearch 2.3.1 Type 1 Reward: Global Signal 2.3.2 Type 2 Reward: Search Step 3 Experiment 3.1 Dataset and Evaluation Metrics 3.2 Baselines 3.3 Training Details 3.4 Main Results 4 Further Analysis 4.1 Different RL Comparison 4.2 Ablation Study 4.3 Case Study 5 Limitations 6 Future Work A Prompt for Research Plan on Question Answering B Experiment Setups C Case Study StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization Ziliang Wang 1∗‡ , Xuhui Zheng 1,2 , Kang An 1,3∗† , Cijun Ouyang 1 , Jialu Cai 1 , Yuhang Wang 1 , Yichao Wu 1 1 SenseTime 2 Nanjing University 3 Shenzhen University {wangziliang1, ouyangcijun, caijialu, wangyuhang, wuyichao}@sensetime.com zhengxuhui@smail.nju.edu.cn, ankang@gml.ac.cn Equal contributionWork done during internship at SenseTime Project leader Corresponding autho…

**Results.** Experiment 3.1 Dataset and Evaluation Metrics 3.2 Baselines 3.3 Training Details 3.4 Main Results 4 Further Analysis 4.1 Different RL Comparison 4.2 Ablation Study 4.3 Case Study 5 Limitations 6 Future Work A Prompt for Research Plan on Question Answering B Experiment Setups C Case Study StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization Ziliang Wang 1∗‡ , Xuhui Zheng 1,2 , Kang An 1,3∗† , Cijun Ouyang 1 , Jialu Cai 1 , Yuhang Wang 1 , Yichao Wu 1 1 SenseTime 2 Nanjing University 3 Shenzhen University {wangziliang1, ouyangcijun, caijialu, wangyuhang, wuyichao}@sensetime.com zhengxuhui@smail.nju.edu.cn, ankang@gml.ac.cn Equal contributionWork done during internship at SenseTime Project leader Corresponding author Abstract Efficient multi-hop reasoning requires Large Language Models (LLMs) based agents to acquire high-value external know…

**Conclusion.** Limitations 6 Future Work A Prompt for Research Plan on Question Answering B Experiment Setups C Case Study StepSearch: Igniting LLMs Search Ability via Step-Wise Proximal Policy Optimization Ziliang Wang 1∗‡ , Xuhui Zheng 1,2 , Kang An 1,3∗† , Cijun Ouyang 1 , Jialu Cai 1 , Yuhang Wang 1 , Yichao Wu 1 1 SenseTime 2 Nanjing University 3 Shenzhen University {wangziliang1, ouyangcijun, caijialu, wangyuhang, wuyichao}@sensetime.com zhengxuhui@smail.nju.edu.cn, ankang@gml.ac.cn Equal contributionWork done during internship at SenseTime Project leader Corresponding author Abstract Efficient multi-hop reasoning requires Large Language Models (LLMs) based agents to acquire high-value external knowledge it…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2505.15107v2.md` · `raw/arxiv/2505.15107v2.fulltext.md`
