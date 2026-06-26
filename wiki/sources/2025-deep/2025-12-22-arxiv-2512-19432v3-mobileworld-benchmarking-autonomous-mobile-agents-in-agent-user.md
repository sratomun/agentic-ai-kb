---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MobileWorld: Benchmarking Autonomous Mobile Agents in Agent-User Interactive and MCP-Augmented Environments"
authors: Quyu Kong, Xu Zhang, Zhenyu Yang, Nolan Gao et al.
url: https://arxiv.org/abs/2512.19432v3
date: 2025-12-22
citationCount: 26
influentialCitationCount: 6
velocity: 4.35
ingested: 2026-06-22
tags: [computer-use-agents, agent-protocols, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MobileWorld: Benchmarking Autonomous Mobile Agents in Agent-User Interactive and MCP-Augmented Environments

**arXiv [2512.19432v3](https://arxiv.org/abs/2512.19432v3)** · 2025-12-22 · **26 citations** (6 influential · 4.35/mo) · Quyu Kong, Xu Zhang, Zhenyu Yang, Nolan Gao et al.

## Abstract
Among existing online mobile-use benchmarks, AndroidWorld has emerged as the dominant benchmark due to its reproducible environment and deterministic evaluation; however, recent agents achieving over 90% success rates indicate its saturation and motivate the need for a more challenging benchmark. In addition, its environment lacks key application categories, such as e-commerce and enterprise communication, and does not reflect realistic mobile-use scenarios characterized by vague user instructions and hybrid tool usage. We introduce MobileWorld, a substantially more challenging benchmark designed to reflect real-world usage through 201 tasks across 20 applications. MobileWorld derives its difficulty from an emphasis on long-horizon, cross-application workflows, requiring nearly twice as many completion steps on average (27.8 vs. 14.3) and featuring a significantly higher proportion of multi-app tasks (62.2% vs. 9.5%) than AndroidWorld. To overcome the limitations of existing environments, MobileWorld achieves a balance between production-grade utility and reproducible evaluation by utilizing open-source alternatives to industry standards (e.g., Mattermost for Slack). This approach enables a fully observable and controlled environment through source code modification and direct backend database access for precise verification. MobileWorld also introduces novel task categories, including agent-user interaction and Model Context Protocol (MCP)-augmented tasks, for evaluating agents in user-aware, hybrid-tool scenarios. To facilitate evaluation, we develop a planner-executor agentic framework with extended action spaces to support user interactions and MCP calls. Our results reveal a sharp performance drop compared to AndroidWorld, with the best agentic framework and end-to-end model achieving 51.7% and 20.9% success rates, respectively, highlighting ample headroom for future research.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Works GUI Agent Benchmarks Agent-User Interaction and MCP-Augmented Benchmarks 3 MobileWorld 3.1 Task Definition GUI-Only Tasks Agent-user Interaction Tasks MCP-augmented Tasks 3.2 Environment Development Action Space Stable and Reproducible Environment Task Evaluation 3.3 Benchmark Construction Task Instructions and Scenarios Agent-User Interaction Task Construction MCP-Augmented Task Construction Human-in-the-Loop Task Validation 3.4 Data Statistics 4 Experiments 4.1 Agentic Framework for MobileWorld 4.2 Metrics 4.3 Experimental Setup 4.4 Main Results 4.5 In-depth Analysis Execution Efficiency User Interaction Quality MCP Tool Integration Completion Step Comparsion with AndroidWorld 4.6 Research Challenge Analysis Challenge 1: Ambiguity Detection and User Engagement Challenge 2: MCP Tool Descriptions and Output Management Challenge 3: Long-Term Memory and State Tracking Challenge 4: Complex Logic Reasoning Challenge 5: Temporal-Spatial Context Awareness 5 Con…

**Method / approach.** methodologies. While these benchmarks have significantly advanced mobile agent research, they face critical limitations summarized in Table ˜ 1 : performance saturation on simpler tasks, the assumption of fully-specified instructions, lack of external tool integration, and a trade-off between realism and deterministic verifiability when using commercial applications. Agent-User Interaction and MCP-Augmented Benchmarks Beyond standard GUI operations, recent work has recognized the importance of evaluating agents on their interaction capabilities and tool usage. τ \tau -bench ( yao2024tau ) introduces dynamic conversations between simulated users and agents equipped with domain-specific API tools and policy guidelines, revealing that even state-of-the-art models like GPT-4o succeed on fewer than 50% of tasks and exhibit low consistency. This highlights the challenge of building agents that can reliably follow rules and handle ambiguous requests. Building on this, τ 2 \tau^{2}…

**Results.** Experiments 4.1 Agentic Framework for MobileWorld 4.2 Metrics 4.3 Experimental Setup 4.4 Main Results 4.5 In-depth Analysis Execution Efficiency User Interaction Quality MCP Tool Integration Completion Step Comparsion with AndroidWorld 4.6 Research Challenge Analysis Challenge 1: Ambiguity Detection and User Engagement Challenge 2: MCP Tool Descriptions and Output Management Challenge 3: Long-Term Memory and State Tracking Challenge 4: Complex Logic Reasoning Challenge 5: Temporal-Spatial Context Awareness 5 Conclusion Future Research Directions A Planner-Executor Agentic Framework Details A.1 Planner A.2 Grounding Executor B APP Information B.1 APP List B.2 Open-source APP Environment Construction Mattermost Mastodon Mail App Taodian App C Case Study C.1 GUI-Only Task Example: Task Completion C.2 GUI-Only Task Example: Information Retrieval C.3…

**Conclusion.** Conclusion Future Research Directions A Planner-Executor Agentic Framework Details A.1 Planner A.2 Grounding Executor B APP Information B.1 APP List B.2 Open-source APP Environment Construction Mattermost Mastodon Mail App Taodian App C Case Study C.1 GUI-Only Task Example: Task Completion C.2 GUI-Only Task Example: Information Retrieval C.3 Agent-User Interaction Task Example C.4 MCP-Augmented Task Example \useunder \ul MobileWorld: Benchmarking Autonomous Mobile Agents in Agent-User Interactive and MCP-Augmented Environments Quyu Kong ∗,1 , Xu Zhang ∗,1 , Zhenyu Yang 2 , Nolan Gao 3 , Chen Liu 1 , Panrong Tong 1 , Chenglin Cai 1 , Hanzhang Zhou 1 , Jianan Zhang 1 , Liangyu Chen 1 , Z…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2512.19432v3.md` · `raw/arxiv/2512.19432v3.fulltext.md`
