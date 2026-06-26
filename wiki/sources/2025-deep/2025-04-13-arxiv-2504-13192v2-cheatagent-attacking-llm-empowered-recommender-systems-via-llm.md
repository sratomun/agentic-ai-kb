---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent"
authors: Liang-bo Ning, Shijie Wang, Wenqi Fan, Qing Li et al.
url: https://arxiv.org/abs/2504.13192v2
date: 2025-04-13
citationCount: 56
influentialCitationCount: 2
velocity: 3.92
ingested: 2026-06-22
tags: [recommendation-agents, agentic-rl, agent-security, agentic-ai, arxiv, 2025, cited]
---

# CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent

**arXiv [2504.13192v2](https://arxiv.org/abs/2504.13192v2)** · 2025-04-13 · **56 citations** (2 influential · 3.92/mo) · Liang-bo Ning, Shijie Wang, Wenqi Fan, Qing Li et al.

## Abstract
Recently, Large Language Model (LLM)-empowered recommender systems (RecSys) have brought significant advances in personalized user experience and have attracted considerable attention. Despite the impressive progress, the research question regarding the safety vulnerability of LLM-empowered RecSys still remains largely under-investigated. Given the security and privacy concerns, it is more practical to focus on attacking the black-box RecSys, where attackers can only observe the system's inputs and outputs. However, traditional attack approaches employing reinforcement learning (RL) agents are not effective for attacking LLM-empowered RecSys due to the limited capabilities in processing complex textual inputs, planning, and reasoning. On the other hand, LLMs provide unprecedented opportunities to serve as attack agents to attack RecSys because of their impressive capability in simulating human-like decision-making processes. Therefore, in this paper, we propose a novel attack framework called CheatAgent by harnessing the human-like capabilities of LLMs, where an LLM-based agent is developed to attack LLM-Empowered RecSys. Specifically, our method first identifies the insertion position for maximum impact with minimal input modification. After that, the LLM agent is designed to generate adversarial perturbations to insert at target positions. To further improve the quality of generated perturbations, we utilize the prompt tuning technique to improve attacking strategies via feedback from the victim RecSys iteratively. Extensive experiments across three real-world datasets demonstrate the effectiveness of our proposed attacking method.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Problem Statement 2.1 Notation and Definitations 2.2 Attacker’s Capabilities 2.3 Attacker’s Objective 3 Methodology 3.1 An Overview of the Proposed CheatAgent 3.2 Insertion Positioning 3.3 LLM Agent-Empowered Perturbation Generation 3.3.1 Initial Policy Generation 3.3.2 Self-Reflection Policy Optimization 3.3.3 Final Perturbation Selection 4 Experiments 4.1 Experimental Details 4.1.1 Datasets . 4.1.2 Victim LLM-based Recommender Systems . 4.1.3 Baselines . 4.1.4 Implementation . 4.1.5 Evaluation Metrics . 4.2 Attack Effectiveness 4.3 Semantic Similarity 4.4 Ablation Study 4.5 Parameter Analysis 5 Related Work 6 Conclusion A Whole process of CheatAgent B Experimental Details B.1 Datasets Statistics B.2 Implementation Details B.3 Additional Experiments C Related Work C.1 LLM-Empowered Recommender Systems C.2 Adversarial Attack for LLM D Discussions CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent Liang-bo Ning The Hong Kong Polytechnic University Hong…

**Method / approach.** Methodology 3.1 An Overview of the Proposed CheatAgent 3.2 Insertion Positioning 3.3 LLM Agent-Empowered Perturbation Generation 3.3.1 Initial Policy Generation 3.3.2 Self-Reflection Policy Optimization 3.3.3 Final Perturbation Selection 4 Experiments 4.1 Experimental Details 4.1.1 Datasets . 4.1.2 Victim LLM-based Recommender Systems . 4.1.3 Baselines . 4.1.4 Implementation . 4.1.5 Evaluation Metrics . 4.2 Attack Effectiveness 4.3 Semantic Similarity 4.4 Ablation Study 4.5 Parameter Analysis 5 Related Work 6 Conclusion A Whole process of CheatAgent B Experimental Details B.1 Datasets Statistics B.2 Implementation Details B.3 Additional Experiments C Related Work C.1 LLM-Empowered Recommender Systems C.2 Adversarial Attack for LLM D Discussions CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent Liang-bo Ning The Hong Kong Polytechnic University Hong Kong China BigLemon1123@gmai…

**Results.** Experiments 4.1 Experimental Details 4.1.1 Datasets . 4.1.2 Victim LLM-based Recommender Systems . 4.1.3 Baselines . 4.1.4 Implementation . 4.1.5 Evaluation Metrics . 4.2 Attack Effectiveness 4.3 Semantic Similarity 4.4 Ablation Study 4.5 Parameter Analysis 5 Related Work 6 Conclusion A Whole process of CheatAgent B Experimental Details B.1 Datasets Statistics B.2 Implementation Details B.3 Additional Experiments C Related Work C.1 LLM-Empowered Recommender Systems C.2 Adversarial Attack for LLM D Discussions CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent Liang-bo Ning The Hong Kong Polytechnic University Hong Kong China BigLemon1123@gmail.com , Shijie Wang The Hong Kong Polytechnic University Hong Kong China shijie.wang@connect.polyu.hk , Wenqi Fan The Hong Kong Polytechnic University Hong Kong China wenqifan03@gmail.…

**Conclusion.** Conclusion A Whole process of CheatAgent B Experimental Details B.1 Datasets Statistics B.2 Implementation Details B.3 Additional Experiments C Related Work C.1 LLM-Empowered Recommender Systems C.2 Adversarial Attack for LLM D Discussions CheatAgent: Attacking LLM-Empowered Recommender Systems via LLM Agent Liang-bo Ning The Hong Kong Polytechnic University Hong Kong China BigLemon1123@gmail.com , Shijie Wang The Hong Kong Polytechnic University Hong Kong China shijie.wang@connect.polyu.hk , Wenqi Fan The Hong Kong Polytechnic University Hong Kong China wenqifan03@gmail.com , Qing Li The Hong Kong Polytechnic University Hong Kong China qing-prof.li@polyu.edu.…

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.13192v2.md` · `raw/arxiv/2504.13192v2.fulltext.md`
