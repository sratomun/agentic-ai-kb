---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "UserBench: An Interactive Gym Environment for User-Centric Agents"
authors: Cheng Qian, Zuxin Liu, Akshara Prabhakar, Zhiwei Liu et al.
url: https://arxiv.org/abs/2507.22034v1
date: 2025-07-29
citationCount: 47
influentialCitationCount: 1
velocity: 4.36
ingested: 2026-06-22
tags: [tool-use, agent-evaluation, arxiv, 2025, cited]
---

# UserBench: An Interactive Gym Environment for User-Centric Agents

**arXiv [2507.22034v1](https://arxiv.org/abs/2507.22034v1)** · 2025-07-29 · **47 citations** (1 influential · 4.36/mo) · Cheng Qian, Zuxin Liu, Akshara Prabhakar, Zhiwei Liu et al.

## Abstract
Large Language Models (LLMs)-based agents have made impressive progress in reasoning and tool use, enabling them to solve complex tasks. However, their ability to proactively collaborate with users, especially when goals are vague, evolving, or indirectly expressed, remains underexplored. To address this gap, we introduce UserBench, a user-centric benchmark designed to evaluate agents in multi-turn, preference-driven interactions. UserBench features simulated users who start with underspecified goals and reveal preferences incrementally, requiring agents to proactively clarify intent and make grounded decisions with tools. Our evaluation of leading open- and closed-source LLMs reveals a significant disconnect between task completion and user alignment. For instance, models provide answers that fully align with all user intents only 20% of the time on average, and even the most advanced models uncover fewer than 30% of all user preferences through active interaction. These results highlight the challenges of building agents that are not just capable task executors, but true collaborative partners. UserBench offers an interactive environment to measure and advance this critical capability.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work User-centric environments for LLM evaluation. User-centric agent designs. 3 UserBench 3.1 Data Gathering 3.2 Tool Augmentation 3.3 Environment Building 3.4 Agent Interaction 3.5 Variants, Scalability and Statistics 4 Experiments 4.1 Settings Gym Settings. Models. Metrics. 4.2 Results Single-choice setting is significantly more challenging. Preference elicitation remains low across models. Understanding users is harder than executing tool use. Other Interesting Findings. 5 Analysis Difficulty tier division effectively reflects UserBench’s challenges. The key challenge lies in the number of preferences per aspect. Models struggle to provide answers that are both correct and timely. More interaction turns do not guarantee better performance. Effect of sampling frequency reveals instability. Less options reduces interference but do not reduce the core challenge. 6 Discussions Broad applicability of UserBench. Balancing efficiency and effectiveness in user interaction. 7 Conclusion…

**Method / approach.** Methods in Natural Language Processing , pages 3102–3116. Li et al. (2025) Xuefeng Li, Haoyang Zou, and Pengfei Liu. 2025. Torl: Scaling tool-integrated rl. arXiv preprint arXiv:2503.23383 . Lin et al. (2024) Bill Yuchen Lin, Yuntian Deng, Khyathi R Chandu, Faeze Brahman, Abhilasha Ravichander, Valentina Pyatkin, Nouha Dziri, Ronan Le Bras, and Yejin Choi. 2024. Wildbench: Benchmarking llms with challenging tasks from real users in the wild. arXiv preprint arXiv:2406.04770 . Liu et al. (2023) Alisa Liu, Zhaofeng Wu, Julian Michael, Alane Suhr, Peter West, Alexander Koller, Swabha Swayamdipta, Noah A Smith, and Yejin Choi. 2023. We’re afraid language models aren’t modeling ambiguity. In The 2023 Conference on Empirical Methods in Natural Language Processing . Liu et al. (2024) Zuxin Liu, Thai Hoang, Jianguo Zhang, Ming Zhu, Tian Lan, Juntao Tan, Weiran Yao, Zhiwei Liu, Yihao Feng, Rithesh RN, et al. 2024. Apigen: Automated pipeline for generating verif…

**Results.** Experiments 4.1 Settings Gym Settings. Models. Metrics. 4.2 Results Single-choice setting is significantly more challenging. Preference elicitation remains low across models. Understanding users is harder than executing tool use. Other Interesting Findings. 5 Analysis Difficulty tier division effectively reflects UserBench’s challenges. The key challenge lies in the number of preferences per aspect. Models struggle to provide answers that are both correct and timely. More interaction turns do not guarantee better performance. Effect of sampling frequency reveals instability. Less options reduces interference but do not reduce the core challenge. 6 Discussions Broad applicability of UserBench. Balancing efficiency and effectiveness in user interaction. 7 Conclusion A Comparison Traits Details B Gym Construction Details Option Generation. Environment Setting. C Experiment…

**Conclusion.** Conclusion A Comparison Traits Details B Gym Construction Details Option Generation. Environment Setting. C Experiment Details Settings. Metrics. D Analysis Details UserBench: An Interactive Gym Environment for User-Centric Agents Cheng Qian 1,2 , Zuxin Liu 1 , Akshara Prabhakar 1 , Zhiwei Liu 1 , Jianguo Zhang 1 , Haolin Chen 1 , Heng Ji 2 , Weiran Yao 1 , Shelby Heinecke 1 , Silvio Savarese 1 , Caiming Xiong 1 , Huan Wang 1 1 Salesforce AI Research 2 University of Illinois Urbana-Champaign Abstract Large Language Models (LLMs)-based agents have made impressive progress in reasoning and tool use, enabling them to solve complex tasks. However, their ability to proactively collaborate with users, esp…

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2507.22034v1.md` · `raw/arxiv/2507.22034v1.fulltext.md`
