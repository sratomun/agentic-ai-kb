---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "SWE-Debate: Competitive Multi-Agent Debate for Software Issue Resolution"
authors: Han Li, Yuling Shi, Shaoxin Lin, Xiaodong Gu et al.
url: https://arxiv.org/abs/2507.23348v1
date: 2025-07-31
citationCount: 44
influentialCitationCount: 2
velocity: 4.11
ingested: 2026-06-22
tags: [coding-agents, agent-reliability, multi-agent-systems, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# SWE-Debate: Competitive Multi-Agent Debate for Software Issue Resolution

**arXiv [2507.23348v1](https://arxiv.org/abs/2507.23348v1)** · 2025-07-31 · **44 citations** (2 influential · 4.11/mo) · Han Li, Yuling Shi, Shaoxin Lin, Xiaodong Gu et al.

## Abstract
Issue resolution has made remarkable progress thanks to the advanced reasoning capabilities of large language models (LLMs). Recently, agent-based frameworks such as SWE-agent have further advanced this progress by enabling autonomous, tool-using agents to tackle complex software engineering tasks. While existing agent-based issue resolution approaches are primarily based on agents' independent explorations, they often get stuck in local solutions and fail to identify issue patterns that span across different parts of the codebase. To address this limitation, we propose SWE-Debate, a competitive multi-agent debate framework that encourages diverse reasoning paths and achieves more consolidated issue localization. SWE-Debate first creates multiple fault propagation traces as localization proposals by traversing a code dependency graph. Then, it organizes a three-round debate among specialized agents, each embodying distinct reasoning perspectives along the fault propagation trace. This structured competition enables agents to collaboratively converge on a consolidated fix plan. Finally, this consolidated fix plan is integrated into an MCTS-based code modification agent for patch generation. Experiments on the SWE-bench benchmark show that SWE-Debate achieves new state-of-the-art results in open-source agent frameworks and outperforms baselines by a large margin.

## From the paper (full-text excerpts)
**Introduction.** INTRODUCTION Automated repository-level issue resolution has emerged as a critical challenge in software engineering. The task aims to automatically localize and fix the defective code snippets, based on reported issues. In software development, developers spend a majority of their debugging efforts in understanding code and making changes [15, 52]. Meanwhile, automated tools often struggle with the same challenge [4, 33, 39]. Inadequate code understanding leads †Equal contribution. ‡ Xiaodong Gu is the corresponding author. 1 Our code and data are available at https://github.com/YerbaPage/SWE-Debate to incomplete fixes, introduces new bugs, and significantly extends development cycles [5, 7]. The key challenge in effective issue resolution is fault localization, namely, identifying the code snippets triggering the specific issue [43]. Unlike conventional code retrieval, fault localization requires a deeper connection between natural language issue descriptions and programming language structures. This process requires reasoning over the structural and semantic properties of code,…

**Method / approach.** methods [1, 3, 38, 46, 52] have emerged, simulating autonomous agents capable of tool use and high-level decision-making. These approaches use iterative exploration and planning to enable systematic codebase traversal, representing a shift toward structured and interactive issue resolution processes [22, 43]. While agent-based approaches have shown notable progress on standard benchmarks such as SWE-bench [15], they mainly rely on agents’ independent exploration, that is, the agents individually understand code repository and propose their modification plans. As a result, they often get stuck in local solutions and fail to identify issue patterns that span across large, complex codebases [5, 7]. This fundamental limitation stems from a core challenge we term limited observation scope [32, 48]: when multiple code locations appear relevant to the issue description, correct resolution often depends on a deep understanding of code structure and component relationships. However, independen…

**Results.** Experiments on the SWE-bench benchmark show that SWE-Debate achieves new state-of-the-art results in open-source agent frameworks and outperforms baselines by a large margin1 . 1 INTRODUCTION Automated repository-level issue resolution has emerged as a critical challenge in software engineering. The task aims to automatically localize and fix the defective code snippets, based on reported issues. In software development, developers spend a majority of their debugging efforts in understanding code and making changes [15, 52]. Meanwhile, automated tools often struggle with the same challenge [4, 33, 39]. Inadequate code understanding leads †Equal contribution. ‡ Xiaodong Gu is the corresponding author. 1 Our code and data are available at https://github.com/YerbaPage/SWE-Debate to incomplete fixes, introduces new bugs, and significantly extends development cycles [5, 7]. The key challenge in effective issue resolution is fault localiz…

**Conclusion.** DISCUSSION 6.1 Strengths SWE-Debate demonstrates three key advantages over existing approaches. First, the graph-based localization significantly improves fault localization accuracy. By building dependency graphs from code structure and generating multiple fault propagation traces, our method achieves 81.67% file-level accuracy. When comparing with SWE-Debate: Competitive Multi-Agent Debate for Software Issue Resolution Conference’17, July 2017, Washington, DC, USA Issue: Evaluating powers of `TensorProduct` Powers of tensor product expressions are not possible to evaluate with either `expand(tensorproduct=True)` method nor the `tensor_product_simp`function. ...... Debate Plan Generate Localization Chain location Chain1： ['physics/…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[swe-bench]]
- **Raw:** `raw/arxiv/2507.23348v1.md` · `raw/arxiv/2507.23348v1.fulltext.md`
