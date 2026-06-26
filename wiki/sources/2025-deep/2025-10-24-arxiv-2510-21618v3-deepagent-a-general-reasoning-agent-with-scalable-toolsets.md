---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DeepAgent: A General Reasoning Agent with Scalable Toolsets"
authors: Xiaoxi Li, Wenxiang Jiao, Jiarui Jin, Guanting Dong et al.
url: https://arxiv.org/abs/2510.21618v3
date: 2025-10-24
citationCount: 50
influentialCitationCount: 3
velocity: 6.32
ingested: 2026-06-22
tags: [agentic-rl, agent-memory, tool-use, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# DeepAgent: A General Reasoning Agent with Scalable Toolsets

**arXiv [2510.21618v3](https://arxiv.org/abs/2510.21618v3)** · 2025-10-24 · **50 citations** (3 influential · 6.32/mo) · Xiaoxi Li, Wenxiang Jiao, Jiarui Jin, Guanting Dong et al.

## Abstract
Large reasoning models have demonstrated strong problem-solving abilities, yet real-world tasks often require external tools and long-horizon interactions. Existing agent frameworks typically follow predefined workflows, which limit autonomous and global task completion. In this paper, we introduce DeepAgent, an end-to-end deep reasoning agent that performs autonomous thinking, tool discovery, and action execution within a single, coherent reasoning process. To manage long-horizon interactions, we introduce an autonomous memory folding mechanism that compresses past interactions into structured episodic, working, and tool memories, reducing error accumulation while preserving critical information. To teach general-purpose tool use efficiently and stably, we develop an end-to-end reinforcement learning strategy, namely ToolPO, that leverages LLM-simulated APIs and applies tool-call advantage attribution to assign fine-grained credit to the tool invocation tokens. Extensive experiments on eight benchmarks, including general tool-use tasks (ToolBench, API-Bank, TMDB, Spotify, ToolHop) and downstream applications (ALFWorld, WebShop, GAIA, HLE), demonstrate that DeepAgent consistently outperforms baselines across both labeled-tool and open-set tool retrieval scenarios. The code and demo are available at https://github.com/RUC-NLPIR/DeepAgent.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Large Reasoning Models 2.2 Autonomous Agents 3 Methodology 3.1 Problem Formulation 3.2 Overview of the DeepAgent Framework 3.3 Autonomous Tool Search and Calling Tool Search Tool Call 3.4 Autonomous Memory Folding and Brain-Inspired Memory Schema 3.5 End-to-end RL Training with ToolPO Training Data Collection Tool Simulator Global and Tool-Call Advantage Attribution Optimization Objective 4 Experimental Settings 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 5 Experimental Results 5.1 Main Results on General Tool Usage Tasks 5.2 Main Results on Downstream Applications 5.3 Analysis of Training Dynamics 5.4 Ablation Studies 5.5 Effectiveness of Tool Retrieval Strategies 5.6 Scaling Analysis of Action Limits 5.7 Generalization Across Different Backbones 6 Conclusion A Datasets A.1 Training Data A.2 Benchmarks General Tool-Use Downstream Applications B Implementation Details C Memory Schema Episodic Memory Schema Working Memory Sch…

**Method / approach.** Methodology 3.1 Problem Formulation 3.2 Overview of the DeepAgent Framework 3.3 Autonomous Tool Search and Calling Tool Search Tool Call 3.4 Autonomous Memory Folding and Brain-Inspired Memory Schema 3.5 End-to-end RL Training with ToolPO Training Data Collection Tool Simulator Global and Tool-Call Advantage Attribution Optimization Objective 4 Experimental Settings 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 5 Experimental Results 5.1 Main Results on General Tool Usage Tasks 5.2 Main Results on Downstream Applications 5.3 Analysis of Training Dynamics 5.4 Ablation Studies 5.5 Effectiveness of Tool Retrieval Strategies 5.6 Scaling Analysis of Action Limits 5.7 Generalization Across Different Backbones 6 Conclusion A Datasets A.1 Training Data A.2 Benchmarks General Tool-Use Downstream Applications B Implementation Details C Memory Schema Episodic Memory Schema Working M…

**Results.** Experimental Settings 4.1 Tasks and Datasets 4.2 Baselines 4.3 Implementation Details 5 Experimental Results 5.1 Main Results on General Tool Usage Tasks 5.2 Main Results on Downstream Applications 5.3 Analysis of Training Dynamics 5.4 Ablation Studies 5.5 Effectiveness of Tool Retrieval Strategies 5.6 Scaling Analysis of Action Limits 5.7 Generalization Across Different Backbones 6 Conclusion A Datasets A.1 Training Data A.2 Benchmarks General Tool-Use Downstream Applications B Implementation Details C Memory Schema Episodic Memory Schema Working Memory Schema Tool Memory Schema D Case Study \useunder \ul \setcctype by-nc-nd DeepAgent: A General Reasoning Agent with Scalable Toolsets Xiaoxi Li Renmin University of China Beijing China xiaoxi˙li@ruc.edu.cn , Wenxiang Jiao , Jiarui Jin Xiaohongshu Inc. Beijing China , Guanting Dong…

**Conclusion.** Conclusion A Datasets A.1 Training Data A.2 Benchmarks General Tool-Use Downstream Applications B Implementation Details C Memory Schema Episodic Memory Schema Working Memory Schema Tool Memory Schema D Case Study \useunder \ul \setcctype by-nc-nd DeepAgent: A General Reasoning Agent with Scalable Toolsets Xiaoxi Li Renmin University of China Beijing China xiaoxi˙li@ruc.edu.cn , Wenxiang Jiao , Jiarui Jin Xiaohongshu Inc. Beijing China , Guanting Dong , Jiajie Jin Renmin University of China Beijing China , Yinuo Wang Tsinghua University Beijing China , Hao Wang Xiaohongshu Inc. Beijing China , Yutao Zhu Renmin University of China…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gaia-benchmark]] · [[alfworld]]
- **Raw:** `raw/arxiv/2510.21618v3.md` · `raw/arxiv/2510.21618v3.fulltext.md`
