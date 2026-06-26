---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Memp: Exploring Agent Procedural Memory"
authors: Runnan Fang, Yuan Liang, Xiaobin Wang, Jialong Wu et al.
url: https://arxiv.org/abs/2508.06433v4
date: 2025-08-08
citationCount: 42
influentialCitationCount: 9
velocity: 4.02
ingested: 2026-06-22
tags: [coding-agents, agent-memory, agentic-ai, arxiv, 2025, cited]
---

# Memp: Exploring Agent Procedural Memory

**arXiv [2508.06433v4](https://arxiv.org/abs/2508.06433v4)** · 2025-08-08 · **42 citations** (9 influential · 4.02/mo) · Runnan Fang, Yuan Liang, Xiaobin Wang, Jialong Wu et al.

## Abstract
Large Language Models (LLMs) based agents excel at diverse tasks, yet they suffer from brittle procedural memory that is manually engineered or entangled in static parameters. In this work, we investigate strategies to endow agents with a learnable, updatable, and lifelong procedural memory. We propose Memp that distills past agent trajectories into both fine-grained, step-by-step instructions and higher-level, script-like abstractions, and explore the impact of different strategies for Build, Retrieval, and Update of procedural memory. Coupled with a dynamic regimen that continuously updates, corrects, and deprecates its contents, this repository evolves in lockstep with new experience. Empirical evaluation on TravelPlanner and ALFWorld shows that as the memory repository is refined, agents achieve steadily higher success rates and greater efficiency on analogous tasks. Moreover, procedural memory built from a stronger model retains its value: migrating the procedural memory to a weaker model can also yield substantial performance gains. Code is available at https://github.com/zjunlp/MemP.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works Memory in Language Agents. Learning from Experience. 3 Preliminary 3.1 Agent Procedural Memory 4 Experiment 4.1 Experimental Settings Datasets. Backbones. 4.2 Memory Storage Retrieval 4.3 Memory Update 4.4 Comparison 5 Analysis Procedural Memory Boosts Accuracy and Cuts Trials. Procedural memory exhibits transferability from strong models to weaker ones. Scaling Memory Retrieval Improves Agent Performance. 6 Conclusion and Future Work References A Use of AI Assistant B Case Study C Evaluation Details License: arXiv.org perpetual non-exclusive license arXiv:2508.06433v4 [cs.CL] 15 Apr 2026 M ​ e ​ m p Mem^{p} : Exploring Agent Procedural Memory Runnan Fang ♠ ♡ ∗ \spadesuit\heartsuit* , Yuan Liang ♠ \spadesuit , Xiaobin Wang ♡ \heartsuit , Jialong Wu ♡ \heartsuit , Shuofei Qiao ♠ ​ ♡ \spadesuit\heartsuit , Pengjun Xie ♡ \heartsuit , Fei Huang ♡ \heartsuit , Huajun Chen ♠ \spadesuit , Ningyu Zhang ♠ ​ ♣ \spadesuit\clubsuit ♠ \spadesuit Zhejiang University ♡ Alibaba Group ♣ \clubsu…

**Method / approach.** methods involve encoding and storing information in various formats, using retrieval mechanisms like vector embeddings and semantic search, and implementing memory updating and forgetting strategies to maintain relevance and efficiency. Despite its importance, memory in multi-turn agent interactions remains underexplored, and enabling agents to effectively learn and utilize memory across trajectories poses a significant challenge. Procedural memory is a type of long-term memory that involves the retention of procedures and skills, such as typing or riding a bike, which are performed automatically without conscious thought. The agent utilizes procedural memory to internalize and automate repetitive tasks, decision-making processes, and interaction patterns, leading to more efficient and context-aware responses over time. Although there have been several works, such as Voyager Wang et al. ( 2023 ) , AWM Wang et al. ( 2024b ) , and AutoManual Chen et al. ( 2024 ) , that utilize proced…

**Results.** Experiment 4.1 Experimental Settings Datasets. Backbones. 4.2 Memory Storage Retrieval 4.3 Memory Update 4.4 Comparison 5 Analysis Procedural Memory Boosts Accuracy and Cuts Trials. Procedural memory exhibits transferability from strong models to weaker ones. Scaling Memory Retrieval Improves Agent Performance. 6 Conclusion and Future Work References A Use of AI Assistant B Case Study C Evaluation Details License: arXiv.org perpetual non-exclusive license arXiv:2508.06433v4 [cs.CL] 15 Apr 2026 M ​ e ​ m p Mem^{p} : Exploring Agent Procedural Memory Runnan Fang ♠ ♡ ∗ \spadesuit\heartsuit* , Yuan Liang ♠ \spadesuit , Xiaobin Wang ♡ \heartsuit , Jialong Wu ♡ \heartsuit , Shuofei Qiao ♠ ​ ♡ \spadesuit\heartsuit , Pengjun Xie ♡ \heartsuit , Fei Huang ♡ \heartsuit , Huajun Chen ♠ \spadesuit , Ningyu Zhang ♠ ​ ♣ \spadesuit\clubsuit ♠ \spadesuit Zhejiang University ♡ Alibaba Group ♣ \cl…

**Conclusion.** Conclusion and Future Work References A Use of AI Assistant B Case Study C Evaluation Details License: arXiv.org perpetual non-exclusive license arXiv:2508.06433v4 [cs.CL] 15 Apr 2026 M ​ e ​ m p Mem^{p} : Exploring Agent Procedural Memory Runnan Fang ♠ ♡ ∗ \spadesuit\heartsuit* , Yuan Liang ♠ \spadesuit , Xiaobin Wang ♡ \heartsuit , Jialong Wu ♡ \heartsuit , Shuofei Qiao ♠ ​ ♡ \spadesuit\heartsuit , Pengjun Xie ♡ \heartsuit , Fei Huang ♡ \heartsuit , Huajun Chen ♠ \spadesuit , Ningyu Zhang ♠ ​ ♣ \spadesuit\clubsuit ♠ \spadesuit Zhejiang University ♡ Alibaba Group ♣ \clubsuit State Key Lab. for Novel Software Technology, Nanjing University, P.R. China {rolnan,zhangningyu}@zju.edu.cn Code: https://github.com…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-memory|Agent memory]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[alfworld]]
- **Raw:** `raw/arxiv/2508.06433v4.md` · `raw/arxiv/2508.06433v4.fulltext.md`
