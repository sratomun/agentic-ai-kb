---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "VerlTool: Towards Holistic Agentic Reinforcement Learning with Tool Use"
authors: Dongfu Jiang, Yi Lu, Zhuofeng Li, Zhiheng Lyu et al.
url: https://arxiv.org/abs/2509.01055v3
date: 2025-09-01
citationCount: 71
influentialCitationCount: 9
velocity: 7.35
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, tool-use, agentic-ai, arxiv, 2025, cited]
---

# VerlTool: Towards Holistic Agentic Reinforcement Learning with Tool Use

**arXiv [2509.01055v3](https://arxiv.org/abs/2509.01055v3)** · 2025-09-01 · **71 citations** (9 influential · 7.35/mo) · Dongfu Jiang, Yi Lu, Zhuofeng Li, Zhiheng Lyu et al.

## Abstract
Reinforcement Learning with Verifiable Rewards (RLVR) has demonstrated success in enhancing LLM reasoning capabilities, but remains limited to single-turn interactions without tool integration. While recent Agentic Reinforcement Learning with Tool use (ARLT) approaches have emerged to address multi-turn tool interactions, existing works develop task-specific codebases that suffer from fragmentation, synchronous execution bottlenecks, and limited extensibility across domains. These inefficiencies hinder broader community adoption and algorithmic innovation. We introduce VerlTool, a unified and modular framework that addresses these limitations through systematic design principles. VerlTool provides four key contributions: (1) upstream alignment with VeRL ensuring compatibility and simplified maintenance, (2) unified tool management via standardized APIs supporting diverse modalities including code execution, search, SQL databases, and vision processing, (3) asynchronous rollout execution achieving near 2$\times$ speedup by eliminating synchronization bottlenecks, and (4) comprehensive evaluation demonstrating competitive performance across 6 ARLT domains. Our framework formalizes ARLT as multi-turn trajectories with multi-modal observation tokens (text/image/video), extending beyond single-turn RLVR paradigms. We train and evaluate models on mathematical reasoning, knowledge QA, SQL generation, visual reasoning, web search, and software engineering tasks, achieving results comparable to specialized systems while providing unified training infrastructure. The modular plugin architecture enables rapid tool integration requiring only lightweight Python definitions, significantly reducing development overhead and providing a scalable foundation for tool-augmented RL research. Our code is open-sourced at https://github.com/TIGER-AI-Lab/verl-tool.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 2.1 Reinforcement Learning for Agentic Tool Use 2.2 Agentic RL Training Frameworks 3 VerlTool Framework 3.1 Preliminaries RLVR 3.2 Agentic Reinforcement Learning with Tool Use ARLT. 3.3 Framework Design Challenges. Overview. Asynchronous Rollout Design. Modular Tool-as-Plugin Design. Tokenization. Parallel Tool Server Backend. 4 Experiments 4.1 Experiment Setup 4.2 Results Training on VerlTool achieves competitive results. Multi-modal tools are well-supported. Dynamics of Tool Usage across Tasks. Emerging behaviours of Agentic RL. 5 Conclusion A Detailed Experiment Setup A.1 Mathematical Reasoning with Python Executor (VT-Math) A.2 Knowledge QA with Search Retriever (VT-Search) A.3 Multi-Turn SQL Query Generation (VT-SQL) A.4 Visual Reasoning with Image Operations (VT-VisualReasoner) A.5 Agentic Web Search (VT-DeeepSearch) A.6 Software Engineering Benchmark (VT-SWE) A.7 Supported Tools A.8 Training and Evaluation Configurations B More related works B.1 Organiza…

**Method / approach.** approaches have emerged to address multi-turn tool interactions, existing works develop task-specific codebases that suffer from fragmentation, synchronous execution bottlenecks, and limited extensibility across domains. These inefficiencies hinder broader community adoption and algorithmic innovation. We introduce Verl Tool , a unified and modular framework that addresses these limitations through systematic design principles. Verl Tool provides four key contributions: (1) upstream alignment with VeRL ensuring compatibility and simplified maintenance, (2) unified tool management via standardized APIs supporting diverse modalities including code execution, search, SQL databases, and vision processing, (3) asynchronous rollout execution achieving near 2 × \times speedup by eliminating synchronization bottlenecks, and (4) comprehensive evaluation demonstrating competitive performance across 6 ARLT domains. Our framework formalizes ARLT as multi-turn trajectories with multi-modal observat…

**Results.** Experiments 4.1 Experiment Setup 4.2 Results Training on VerlTool achieves competitive results. Multi-modal tools are well-supported. Dynamics of Tool Usage across Tasks. Emerging behaviours of Agentic RL. 5 Conclusion A Detailed Experiment Setup A.1 Mathematical Reasoning with Python Executor (VT-Math) A.2 Knowledge QA with Search Retriever (VT-Search) A.3 Multi-Turn SQL Query Generation (VT-SQL) A.4 Visual Reasoning with Image Operations (VT-VisualReasoner) A.5 Agentic Web Search (VT-DeeepSearch) A.6 Software Engineering Benchmark (VT-SWE) A.7 Supported Tools A.8 Training and Evaluation Configurations B More related works B.1 Organization B.2 Tool-Integrated Reasoning B.3 From Tool Integration to Agentic LLMs Agentic LLMs. Agentic Tool-calling Acquisition. B.4 Reinforcement Learning with Verifiable Reward (RLVR) B.5 Agentic Reinforcement Learning with Tool Use (ARLT)…

**Conclusion.** Conclusion A Detailed Experiment Setup A.1 Mathematical Reasoning with Python Executor (VT-Math) A.2 Knowledge QA with Search Retriever (VT-Search) A.3 Multi-Turn SQL Query Generation (VT-SQL) A.4 Visual Reasoning with Image Operations (VT-VisualReasoner) A.5 Agentic Web Search (VT-DeeepSearch) A.6 Software Engineering Benchmark (VT-SWE) A.7 Supported Tools A.8 Training and Evaluation Configurations B More related works B.1 Organization B.2 Tool-Integrated Reasoning B.3 From Tool Integration to Agentic LLMs Agentic LLMs. Agentic Tool-calling Acquisition. B.4 Reinforcement Learning with Verifiable Reward (RLVR) B.5 Agentic Reinforcement Learning with Tool Use (ARLT) Mathematical Interactive…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2509.01055v3.md` · `raw/arxiv/2509.01055v3.fulltext.md`
