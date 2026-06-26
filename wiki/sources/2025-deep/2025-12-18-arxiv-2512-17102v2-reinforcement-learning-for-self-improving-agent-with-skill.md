---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Reinforcement Learning for Self-Improving Agent with Skill Library"
authors: Jiongxiao Wang, Qiaojing Yan, Yawei Wang, Yijun Tian et al.
url: https://arxiv.org/abs/2512.17102v2
date: 2025-12-18
citationCount: 47
influentialCitationCount: 1
velocity: 7.69
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agent-skills, agentic-ai, arxiv, 2025, cited]
---

# Reinforcement Learning for Self-Improving Agent with Skill Library

**arXiv [2512.17102v2](https://arxiv.org/abs/2512.17102v2)** · 2025-12-18 · **47 citations** (1 influential · 7.69/mo) · Jiongxiao Wang, Qiaojing Yan, Yawei Wang, Yijun Tian et al.

## Abstract
Large Language Model (LLM)-based agents have demonstrated remarkable capabilities in complex reasoning and multi-turn interactions but struggle to continuously improve and adapt when deployed in new environments. One promising approach is implementing skill libraries that allow agents to learn, validate, and apply new skills. However, current skill library approaches rely primarily on LLM prompting, making consistent skill library implementation challenging. To overcome these challenges, we propose a Reinforcement Learning (RL)-based approach to enhance agents' self-improvement capabilities with a skill library. Specifically, we introduce Skill Augmented GRPO for self-Evolution (SAGE), a novel RL framework that systematically incorporates skills into learning. The framework's key component, Sequential Rollout, iteratively deploys agents across a chain of similar tasks for each rollout. As agents navigate through the task chain, skills generated from previous tasks accumulate in the library and become available for subsequent tasks. Additionally, the framework enhances skill generation and utilization through a Skill-integrated Reward that complements the original outcome-based rewards. Experimental results on AppWorld demonstrate that SAGE, when applied to supervised-finetuned model with expert experience, achieves 8.9% higher Scenario Goal Completion while requiring 26% fewer interaction steps and generating 59% fewer tokens, substantially outperforming existing approaches in both accuracy and efficiency.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Method 3.1 Skill Library Agent 3.2 SAGE for Skill Library Agent 3.2.1 Preliminary 3.2.2 Sequential Rollout 3.2.3 Skill-integrated Reward 3.2.4 SAGE 4 Experiments 4.1 Experimental Settings 4.2 Main Results 4.3 Skill Library Usage Analysis 4.4 Ablation Studies 5 Conclusion References A Interaction Format Example of Skill Library Agent B SAGE with Longer Task Chain in Sequential Rollout C AppWorld Dataset D Prompt for Skill Library Agent E Training Details of Baseline GRPO F Expert Experience Dataset Generation G Training Details of SAGE H Task Execution Examples with Different Models I Retrieval Method Ablation Study I.1 Details of Retrieval Methods I.2 Further Analysis J Reward Design Ablation Study J.1 Details of Reward Designs J.2 Skill Library Usage Analysis K RL Initialization Methods L SFT Initialized Baseline GRPO License: arXiv.org perpetual non-exclusive license arXiv:2512.17102v2 [cs.AI] 10 Mar 2026 Reinforcement Learning for Self-Improving Agent with Skill L…

**Method / approach.** Method 3.1 Skill Library Agent 3.2 SAGE for Skill Library Agent 3.2.1 Preliminary 3.2.2 Sequential Rollout 3.2.3 Skill-integrated Reward 3.2.4 SAGE 4 Experiments 4.1 Experimental Settings 4.2 Main Results 4.3 Skill Library Usage Analysis 4.4 Ablation Studies 5 Conclusion References A Interaction Format Example of Skill Library Agent B SAGE with Longer Task Chain in Sequential Rollout C AppWorld Dataset D Prompt for Skill Library Agent E Training Details of Baseline GRPO F Expert Experience Dataset Generation G Training Details of SAGE H Task Execution Examples with Different Models I Retrieval Method Ablation Study I.1 Details of Retrieval Methods I.2 Further Analysis J Reward Design Ablation Study J.1 Details of Reward Designs J.2 Skill Library Usage Analysis K RL Initialization Methods L SFT Initialized Baseline GRPO License: arXiv.org perpetual non-exclusive license arXiv:2512.17102v2 [cs.AI] 10 Mar 202…

**Results.** Experiments 4.1 Experimental Settings 4.2 Main Results 4.3 Skill Library Usage Analysis 4.4 Ablation Studies 5 Conclusion References A Interaction Format Example of Skill Library Agent B SAGE with Longer Task Chain in Sequential Rollout C AppWorld Dataset D Prompt for Skill Library Agent E Training Details of Baseline GRPO F Expert Experience Dataset Generation G Training Details of SAGE H Task Execution Examples with Different Models I Retrieval Method Ablation Study I.1 Details of Retrieval Methods I.2 Further Analysis J Reward Design Ablation Study J.1 Details of Reward Designs J.2 Skill Library Usage Analysis K RL Initialization Methods L SFT Initialized Baseline GRPO License: arXiv.org perpetual non-exclusive license arXiv:2512.17102v2 [cs.AI] 10 Mar 2026 Reinforcement Learning for Self-Improving Agent with Skill Library Jiongxiao Wang 1 Qiaojing Yan 2 Yawei Wang 2…

**Conclusion.** Conclusion References A Interaction Format Example of Skill Library Agent B SAGE with Longer Task Chain in Sequential Rollout C AppWorld Dataset D Prompt for Skill Library Agent E Training Details of Baseline GRPO F Expert Experience Dataset Generation G Training Details of SAGE H Task Execution Examples with Different Models I Retrieval Method Ablation Study I.1 Details of Retrieval Methods I.2 Further Analysis J Reward Design Ablation Study J.1 Details of Reward Designs J.2 Skill Library Usage Analysis K RL Initialization Methods L SFT Initialized Baseline GRPO License: arXiv.org perpetual non-exclusive license arXiv:2512.17102v2 [cs.AI] 10 Mar 2026 Reinforcement Learning for Self-Improving…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2512.17102v2.md` · `raw/arxiv/2512.17102v2.fulltext.md`
