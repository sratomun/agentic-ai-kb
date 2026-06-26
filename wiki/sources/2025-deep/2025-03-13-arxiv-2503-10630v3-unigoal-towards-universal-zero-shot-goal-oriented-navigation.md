---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "UniGoal: Towards Universal Zero-shot Goal-oriented Navigation"
authors: Hang Yin, Xiuwei Xu, Lingqing Zhao, Ziwei Wang et al.
url: https://arxiv.org/abs/2503.10630v3
date: 2025-03-13
citationCount: 78
influentialCitationCount: 11
velocity: 5.1
ingested: 2026-06-22
tags: [embodied-agents, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# UniGoal: Towards Universal Zero-shot Goal-oriented Navigation

**arXiv [2503.10630v3](https://arxiv.org/abs/2503.10630v3)** · 2025-03-13 · **78 citations** (11 influential · 5.1/mo) · Hang Yin, Xiuwei Xu, Lingqing Zhao, Ziwei Wang et al.

## Abstract
In this paper, we propose a general framework for universal zero-shot goal-oriented navigation. Existing zero-shot methods build inference framework upon large language models (LLM) for specific tasks, which differs a lot in overall pipeline and fails to generalize across different types of goal. Towards the aim of universal zero-shot navigation, we propose a uniform graph representation to unify different goals, including object category, instance image and text description. We also convert the observation of agent into an online maintained scene graph. With this consistent scene and goal representation, we preserve most structural information compared with pure text and are able to leverage LLM for explicit graph-based reasoning. Specifically, we conduct graph matching between the scene graph and goal graph at each time instant and propose different strategies to generate long-term goal of exploration according to different matching states. The agent first iteratively searches subgraph of goal when zero-matched. With partial matching, the agent then utilizes coordinate projection and anchor pair alignment to infer the goal location. Finally scene graph correction and goal verification are applied for perfect matching. We also present a blacklist mechanism to enable robust switch between stages. Extensive experiments on several benchmarks show that our UniGoal achieves state-of-the-art zero-shot performance on three studied navigation tasks with a single model, even outperforming task-specific zero-shot methods and supervised universal methods.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Approach 3.1 Goal-oriented Navigation 3.2 Graph Construction and Matching 3.3 Multi-stage Scene Exploration 3.4 Robust Blacklist Mechanism 4 Experiments 4.1 Benchmarks and Implementation Details 4.2 Comparison with State-of-the-art 4.3 Ablation Study 4.4 Qualitative Results 5 Conclusion A Overview B Definition of Each Task C Pipeline of UniGoal D Details of Approach D.1 Goal Graph Construction D.2 Graph Embedding D.3 Zero Matching D.4 Hyperparameters E Prompts \newmdenv [ backgroundcolor=verylightgray, hidealllines=true, innerleftmargin=8pt, innerrightmargin=8pt, innertopmargin=2pt, innerbottommargin=4pt ]graybox UniGoal: Towards Universal Zero-shot Goal-oriented Navigation Hang Yin 1 , Xiuwei Xu 1∗† , Linqing Zhao 1 , Ziwei Wang 2 , Jie Zhou 1 , Jiwen Lu 1‡ 1 Tsinghua University 2 Nanyang Technological University {yinh23, xxw21, zhaolinqing}@mails.tsinghua.edu.cn; ziwei.wang@ntu.edu.sg; {jzhou, lujiwen}@tsinghua.edu.cn Equal contribution. † Project lead. ‡ Corresponding author.…

**Method / approach.** methods build inference framework upon large language models (LLM) for specific tasks, which differs a lot in overall pipeline and fails to generalize across different types of goal. Towards the aim of universal zero-shot navigation, we propose a uniform graph representation to unify different goals, including object category, instance image and text description. We also convert the observation of agent into an online maintained scene graph. With this consistent scene and goal representation, we preserve most structural information compared with pure text and are able to leverage LLM for explicit graph-based reasoning. Specifically, we conduct graph matching between the scene graph and goal graph at each time instant and propose different strategies to generate long-term goal of exploration according to different matching states. The agent first iteratively searches subgraph of goal when zero-matched. With partial matching, the agent then utilizes coordinate projection and anchor pair…

**Results.** Experiments 4.1 Benchmarks and Implementation Details 4.2 Comparison with State-of-the-art 4.3 Ablation Study 4.4 Qualitative Results 5 Conclusion A Overview B Definition of Each Task C Pipeline of UniGoal D Details of Approach D.1 Goal Graph Construction D.2 Graph Embedding D.3 Zero Matching D.4 Hyperparameters E Prompts \newmdenv [ backgroundcolor=verylightgray, hidealllines=true, innerleftmargin=8pt, innerrightmargin=8pt, innertopmargin=2pt, innerbottommargin=4pt ]graybox UniGoal: Towards Universal Zero-shot Goal-oriented Navigation Hang Yin 1 , Xiuwei Xu 1∗† , Linqing Zhao 1 , Ziwei Wang 2 , Jie Zhou 1 , Jiwen Lu 1‡ 1 Tsinghua University 2 Nanyang Technological University {yinh23, xxw21, zhaolinqing}@mails.tsinghua.edu.cn; ziwei.wang@ntu.edu.sg; {jzhou, lujiwen}@tsinghua.edu.cn Equal contribution. † Project lead. ‡ Corresponding author. Abstract In this paper, we propose…

**Conclusion.** Conclusion A Overview B Definition of Each Task C Pipeline of UniGoal D Details of Approach D.1 Goal Graph Construction D.2 Graph Embedding D.3 Zero Matching D.4 Hyperparameters E Prompts \newmdenv [ backgroundcolor=verylightgray, hidealllines=true, innerleftmargin=8pt, innerrightmargin=8pt, innertopmargin=2pt, innerbottommargin=4pt ]graybox UniGoal: Towards Universal Zero-shot Goal-oriented Navigation Hang Yin 1 , Xiuwei Xu 1∗† , Linqing Zhao 1 , Ziwei Wang 2 , Jie Zhou 1 , Jiwen Lu 1‡ 1 Tsinghua University 2 Nanyang Technological University {yinh23, xxw21, zhaolinqing}@mails.tsinghua.edu.cn; ziwei.wang@ntu.edu.sg; {jzhou, lujiwen}@tsinghua.edu.cn Equal contribution. † Project lead. ‡ Correspond…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2503.10630v3.md` · `raw/arxiv/2503.10630v3.fulltext.md`
