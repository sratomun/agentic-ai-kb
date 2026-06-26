---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers"
authors: Ziyang Luo, Zhiqi Shen, Wenzhuo Yang, Zirui Zhao et al.
url: https://arxiv.org/abs/2508.14704v1
date: 2025-08-20
citationCount: 77
influentialCitationCount: 14
velocity: 7.66
ingested: 2026-06-22
tags: [coding-agents, embodied-agents, finance-agents, agent-protocols, agent-memory, arxiv, 2025, cited]
---

# MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers

**arXiv [2508.14704v1](https://arxiv.org/abs/2508.14704v1)** · 2025-08-20 · **77 citations** (14 influential · 7.66/mo) · Ziyang Luo, Zhiqi Shen, Wenzhuo Yang, Zirui Zhao et al.

## Abstract
The Model Context Protocol has emerged as a transformative standard for connecting large language models to external data sources and tools, rapidly gaining adoption across major AI providers and development platforms. However, existing benchmarks are overly simplistic and fail to capture real application challenges such as long-horizon reasoning and large, unfamiliar tool spaces. To address this critical gap, we introduce MCP-Universe, the first comprehensive benchmark specifically designed to evaluate LLMs in realistic and hard tasks through interaction with real-world MCP servers. Our benchmark encompasses 6 core domains spanning 11 different MCP servers: Location Navigation, Repository Management, Financial Analysis, 3D Design, Browser Automation, and Web Searching. To ensure rigorous evaluation, we implement execution-based evaluators, including format evaluators for agent format compliance, static evaluators for time-invariant content matching, and dynamic evaluators that automatically retrieve real-time ground truth for temporally sensitive tasks. Through extensive evaluation of leading LLMs, we find that even SOTA models such as GPT-5 (43.72%), Grok-4 (33.33%) and Claude-4.0-Sonnet (29.44%) exhibit significant performance limitations. In addition, our benchmark poses a significant long-context challenge for LLM agents, as the number of input tokens increases rapidly with the number of interaction steps. Moreover, it introduces an unknown-tools challenge, as LLM agents often lack familiarity with the precise usage of the MCP servers. Notably, enterprise-level agents like Cursor cannot achieve better performance than standard ReAct frameworks. Beyond evaluation, we open-source our extensible evaluation framework with UI support, enabling researchers and practitioners to seamlessly integrate new agents and MCP servers while fostering innovation in the rapidly evolving MCP ecosystem.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 MCP-Universe 3.1 Overview 3.2 Evaluation Framework 3.3 Real-World MCP Servers 3.4 Tasks and Evaluators 4 Experiment 4.1 Setup 4.2 Frontier Models Performance 4.3 Long Context Challenges 4.4 Unknown Tools Challenges 4.5 More MCP Servers Connected 4.6 Enterprise-Level Agent Framework Comparison 5 Conclusion A MCP Servers B Tasks and Evaluators Examples C Setup D Naive Error E Summarization Agent F Exploration Agent \shadowtext MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers Ziyang Luo 1 1 footnotemark: 1 Zhiqi Shen 1 1 footnotemark: 1 Wenzhuo Yang 1 1 footnotemark: 1 Zirui Zhao Prathyusha Jwalapuram Amrita Saha Doyen Sahoo Silvio Savarese Caiming Xiong Junnan Li Salesforce AI Research \faGithub https://github.com/SalesforceAIResearch/MCP-Universe \faGlobe https://mcp-universe.github.io Equal Contributions. Abstract The Model Context Protocol (MCP) has emerged as a transformative standard for connecting large lang…

**Method / approach.** methods are insufficient to address these issues. As such, our benchmark serves as a valuable testbed for evaluating and developing long context handling in LLM agent systems. 4.4 Unknown Tools Challenges Figure 5: (Left) An example of the unknown tool challenges. (Right) Effect of introducing the exploration phase on LLM agent performance across selected domains. In addition to the long context challenges, our error analysis reveals that LLMs often struggle to correctly use tools provided by the MCP servers, indicating a lack of familiarity with their interfaces and constraints. For example, Figure 5 (left) illustrates a common failure in the Yahoo Finance MCP server: retrieving a stock price requires specifying a start and end date that differ, yet LLMs frequently set them to be identical, leading to execution errors. To address this issue, we introduce an additional step called the exploration phase. During this phase, the LLM is allowed to freely interact with the tools…

**Results.** Experiment 4.1 Setup 4.2 Frontier Models Performance 4.3 Long Context Challenges 4.4 Unknown Tools Challenges 4.5 More MCP Servers Connected 4.6 Enterprise-Level Agent Framework Comparison 5 Conclusion A MCP Servers B Tasks and Evaluators Examples C Setup D Naive Error E Summarization Agent F Exploration Agent \shadowtext MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers Ziyang Luo 1 1 footnotemark: 1 Zhiqi Shen 1 1 footnotemark: 1 Wenzhuo Yang 1 1 footnotemark: 1 Zirui Zhao Prathyusha Jwalapuram Amrita Saha Doyen Sahoo Silvio Savarese Caiming Xiong Junnan Li Salesforce AI Research \faGithub https://github.com/SalesforceAIResearch/MCP-Universe \faGlobe https://mcp-universe.github.io Equal Contributions. Abstract The Model Context Protocol (MCP) has emerged as a transformative standard for connecting large language…

**Conclusion.** Conclusion A MCP Servers B Tasks and Evaluators Examples C Setup D Naive Error E Summarization Agent F Exploration Agent \shadowtext MCP-Universe: Benchmarking Large Language Models with Real-World Model Context Protocol Servers Ziyang Luo 1 1 footnotemark: 1 Zhiqi Shen 1 1 footnotemark: 1 Wenzhuo Yang 1 1 footnotemark: 1 Zirui Zhao Prathyusha Jwalapuram Amrita Saha Doyen Sahoo Silvio Savarese Caiming Xiong Junnan Li Salesforce AI Research \faGithub https://github.com/SalesforceAIResearch/MCP-Universe \faGlobe https://mcp-universe.github.io Equal Contributions. Abstract The Model Context Protocol (MCP) has emerged as a transformative standard for connecting large language models…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]] · [[finance-agents|Finance agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]]
- **Entities:** [[mcp]] · [[claude]] · [[gpt-5]]
- **Raw:** `raw/arxiv/2508.14704v1.md` · `raw/arxiv/2508.14704v1.fulltext.md`
