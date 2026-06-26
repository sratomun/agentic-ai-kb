---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills"
authors: Boyuan Zheng, Michael Y. Fatemi, Xiaolong Jin, Zora Zhiruo Wang et al.
url: https://arxiv.org/abs/2504.07079v1
date: 2025-04-09
citationCount: 85
influentialCitationCount: 7
velocity: 5.89
ingested: 2026-06-22
tags: [computer-use-agents, self-evolving-agents, agent-skills, agentic-ai, arxiv, 2025, cited]
---

# SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills

**arXiv [2504.07079v1](https://arxiv.org/abs/2504.07079v1)** · 2025-04-09 · **85 citations** (7 influential · 5.89/mo) · Boyuan Zheng, Michael Y. Fatemi, Xiaolong Jin, Zora Zhiruo Wang et al.

## Abstract
To survive and thrive in complex environments, humans have evolved sophisticated self-improvement mechanisms through environment exploration, hierarchical abstraction of experiences into reuseable skills, and collaborative construction of an ever-growing skill repertoire. Despite recent advancements, autonomous web agents still lack crucial self-improvement capabilities, struggling with procedural knowledge abstraction, refining skills, and skill composition. In this work, we introduce SkillWeaver, a skill-centric framework enabling agents to self-improve by autonomously synthesizing reusable skills as APIs. Given a new website, the agent autonomously discovers skills, executes them for practice, and distills practice experiences into robust APIs. Iterative exploration continually expands a library of lightweight, plug-and-play APIs, significantly enhancing the agent's capabilities. Experiments on WebArena and real-world websites demonstrate the efficacy of SkillWeaver, achieving relative success rate improvements of 31.8% and 39.8%, respectively. Additionally, APIs synthesized by strong agents substantially enhance weaker agents through transferable skills, yielding improvements of up to 54.3% on WebArena. These results demonstrate the effectiveness of honing diverse website interactions into APIs, which can be seamlessly shared among various web agents.

## From the paper (full-text excerpts)
**Introduction.** Introduction AI agents based on large language models (LLMs) that can browse the web (Deng et al., 2023; Zhou et al., 2024a; Zheng et al., 2024) or use computers (Xie et al., 2024) like humans are rapidly rising as a new frontier of AI research and application. Despite these promising opportunities, digital environments present substantial challenges due to their inherent complexity and diversity. Website environments are highly intricate, consisting of numerous interactive elements that create large action spaces. An even greater challenge lies in developing generalist web agents capable of generalizing to out-of-distribution task types and adapting to novel websites. Existing efforts have attempted to train web agents using large-scale trajectory datasets collected across diverse websites and task types (Li et al., 2024; Pahuja et al., 2025). However, these agents often struggle with overfitting to specific website structures and task distributions (Li et al., 2024; Zheng et al., 2024), reducing their ability to handle previously unseen environments effectively. As an integral fea…

**Method / approach.** methods typically store skills implicitly through action trajectories, primarily leveraging them as demonstrations for in-context learning (Murty et al., 2024b) or fine-tuning (Murty et al., 2024a; Su et al., 2025; Pahuja et al., 2025). Although these trajectory-based approaches can be effective, they struggle to explicitly abstract reusable procedural knowledge, resulting in heavy training demands and limited generalization to new websites and tasks. Furthermore, continuously updating models with new trajectories introduces significant concerns such as catastrophic forgetting and sensitivity to website changes. Additionally, storing and sharing extensive memory-intensive trajectory data also poses practical challenges for knowledge transfer among agents.2 Efforts like Agent Workflow Memory (Wang et al., 2024e) and ICAL (Sarch et al., 2024) take this a step further by generating abstract, reusable routines. However, its natural language-based routines pose challenges for formal verifi…

**Results.** Experiments on WebArena and real-world websites demonstrate the efficacy of S KILLW EAVER, achieving relative success rate improvements of 31.8% and 39.8%, respectively. Additionally, APIs synthesized by strong agents substantially enhance weaker agents through transferable skills, yielding improvements of up to 54.3% on WebArena. These results demonstrate the effectiveness of honing diverse website interactions into APIs, which can be seamlessly shared among various web agents.1 1 Introduction AI agents based on large language models (LLMs) that can browse the web (Deng et al., 2023; Zhou et al., 2024a; Zheng et al., 2024) or use computers (Xie et al., 2024) like humans are rapidly rising as a new frontier of AI research and application. Despite these promising opportunities, digital environments present substantial challenges due to their inherent complexity and diversity. Website environments are highly intricate, consisting of nu…

**Conclusion.** Conclusion Web agents aim to automate browsing tasks to enhance human productivity across diverse digital environments. A key challenge lies in adapting to real-world websites characterized by high diversity and complexity. Inspired by the self-improvement mechanism of humans, we propose S KILLW EAVER, a skill-centric framework that enables web agents to autonomously self-improve through exploration and API synthesis. Experimental results demonstrate substantial performance improvements, with relative success rate gains of 31.8% on WebArena benchmark and 39.8% on real-world websites. Notably, weaker agents 9 equipped with skills from more powerful counterparts showed improvements of up to 54.3%, demonstrating effective knowledge distilla…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[webarena]]
- **Raw:** `raw/arxiv/2504.07079v1.md` · `raw/arxiv/2504.07079v1.fulltext.md`
