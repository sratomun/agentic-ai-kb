---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Inducing Programmatic Skills for Agentic Tasks"
authors: Zora Zhiruo Wang, Apurva Gandhi, Graham Neubig, Daniel Fried
url: https://arxiv.org/abs/2504.06821v2
date: 2025-04-09
citationCount: 62
influentialCitationCount: 3
velocity: 4.3
ingested: 2026-06-22
tags: [computer-use-agents, embodied-agents, agent-skills, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# Inducing Programmatic Skills for Agentic Tasks

**arXiv [2504.06821v2](https://arxiv.org/abs/2504.06821v2)** · 2025-04-09 · **62 citations** (3 influential · 4.3/mo) · Zora Zhiruo Wang, Apurva Gandhi, Graham Neubig, Daniel Fried

## Abstract
To succeed in common digital tasks such as web navigation, agents must carry out a variety of specialized tasks such as searching for products or planning a travel route. To tackle these tasks, agents can bootstrap themselves by learning task-specific skills online through interaction with the web environment. In this work, we demonstrate that programs are an effective representation for skills. We propose agent skill induction (ASI), which allows agents to adapt themselves by inducing, verifying, and utilizing program-based skills on the fly. We start with an evaluation on the WebArena agent benchmark and show that ASI outperforms the static baseline agent and its text-skill counterpart by 23.5% and 11.3% in success rate, mainly thanks to the programmatic verification guarantee during the induction phase. ASI also improves efficiency by reducing 10.7-15.3% of the steps over baselines, by composing primitive actions (e.g., click) into higher-level skills (e.g., search product). We then highlight the efficacy of ASI in remaining efficient and accurate under scaled-up web activities. Finally, we examine the generalizability of induced skills when transferring between websites, and find that ASI can effectively reuse common skills, while also updating incompatible skills to versatile website changes.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Agent Skill Induction 2.1 Problem Statement: Online Adaptive Agent 2.2 Inducing Reusable Skills 2.3 Inducing and Verifying Programmatic Skills 3 General Web Navigation Performance 3.1 Experiment Setup 3.2 Results and Analysis 3.3 Why are Programmatic Skills Better? 4 Scaled-Up Browsing Activities 5 Adapting Across Websites 6 Related Work 7 Conclusion and Future Discussions A Experiment Details A.1 Agent Action Space A.2 Prompts for LLM-Based Components B Skill Induction: Analysis B.1 Skill Induction and Reusability B.2 Representative Skills Chaining Primitive Actions Advanced Programming Primitives C Scaled-Up and Cross-Website Tests C.1 Scaled-Up Tasks C.2 Cross-Website Tasks C.3 Significance Testing Scaled-Up Tasks Cross-Web Tasks \addauthor dfcyan \addauthor gnmagenta \addauthor zworange \addauthor agbrown Inducing Programmatic Skills for Agentic Tasks Zora Zhiruo Wang Apurva Gandhi Graham Neubig Daniel Fried Carnegie Mellon University {zhiruow,apurvag,gneubig,dfried}…

**Method / approach.** method. Because AWM was originally developed with the gpt-4o model, for a fairer comparison, we also experiment with AWM with claude-3.5-sonnet model as its LM backbone and also apply the episode cleaning procedure to enhance induction quality. We compare the two baseline methods with our ASI approach. We provide the complete prompts for each agent component: task-solving, episode evaluation, episode cleaning, and skill induction, in § A . 3.2 Results and Analysis Model Method # Steps SR Shop Admin Reddit GitLab Maps Multi GPT Vanilla - 12.3 13.9 10.4 6.6 15.0 15.6 8.3 AWM 5.9 35.5 32.1 29.1 54.7 35.0 42.2 18.8 Claude Vanilla 5.6 32.7 32.6 36.8 36.8 26.1 38.5 20.8 AWM 5.9 36.3 34.8 39.0 51.9 28.9 39.4 18.8 ASI (ours) 5.0 40.4 40.1 44.0 54.7 32.2 43.1 20.8 Table 1: WebArena success rate by adaptive agents with programmatic skills, in comparison to a static v…

**Results.** Experiment Setup 3.2 Results and Analysis 3.3 Why are Programmatic Skills Better? 4 Scaled-Up Browsing Activities 5 Adapting Across Websites 6 Related Work 7 Conclusion and Future Discussions A Experiment Details A.1 Agent Action Space A.2 Prompts for LLM-Based Components B Skill Induction: Analysis B.1 Skill Induction and Reusability B.2 Representative Skills Chaining Primitive Actions Advanced Programming Primitives C Scaled-Up and Cross-Website Tests C.1 Scaled-Up Tasks C.2 Cross-Website Tasks C.3 Significance Testing Scaled-Up Tasks Cross-Web Tasks \addauthor dfcyan \addauthor gnmagenta \addauthor zworange \addauthor agbrown Inducing Programmatic Skills for Agentic Tasks Zora Zhiruo Wang Apurva Gandhi Graham Neubig Daniel Fried Carnegie Mellon University {zhiruow,apurvag,gneubig,dfried}@cs.cmu.edu Abstract To succeed in common digital tasks such as…

**Conclusion.** Conclusion and Future Discussions A Experiment Details A.1 Agent Action Space A.2 Prompts for LLM-Based Components B Skill Induction: Analysis B.1 Skill Induction and Reusability B.2 Representative Skills Chaining Primitive Actions Advanced Programming Primitives C Scaled-Up and Cross-Website Tests C.1 Scaled-Up Tasks C.2 Cross-Website Tasks C.3 Significance Testing Scaled-Up Tasks Cross-Web Tasks \addauthor dfcyan \addauthor gnmagenta \addauthor zworange \addauthor agbrown Inducing Programmatic Skills for Agentic Tasks Zora Zhiruo Wang Apurva Gandhi Graham Neubig Daniel Fried Carnegie Mellon University {zhiruow,apurvag,gneubig,dfried}@cs.cmu.edu Abstract To succeed in…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-skills|Agent skills]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[webarena]]
- **Raw:** `raw/arxiv/2504.06821v2.md` · `raw/arxiv/2504.06821v2.fulltext.md`
