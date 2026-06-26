---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Deep Research Agents: A Systematic Examination And Roadmap"
authors: Yuxuan Huang, Yihang Chen, Haozheng Zhang, Kang Li et al.
url: https://arxiv.org/abs/2506.18096v2
date: 2025-06-22
citationCount: 107
influentialCitationCount: 6
velocity: 8.92
ingested: 2026-06-22
tags: [coding-agents, science-agents, agent-protocols, agent-memory, tool-use, arxiv, 2025, cited]
---

# Deep Research Agents: A Systematic Examination And Roadmap

**arXiv [2506.18096v2](https://arxiv.org/abs/2506.18096v2)** · 2025-06-22 · **107 citations** (6 influential · 8.92/mo) · Yuxuan Huang, Yihang Chen, Haozheng Zhang, Kang Li et al.

## Abstract
The rapid progress of Large Language Models (LLMs) has given rise to a new category of autonomous AI systems, referred to as Deep Research (DR) agents. These agents are designed to tackle complex, multi-turn informational research tasks by leveraging a combination of dynamic reasoning, adaptive long-horizon planning, multi-hop information retrieval, iterative tool use, and the generation of structured analytical reports. In this paper, we conduct a detailed analysis of the foundational technologies and architectural components that constitute Deep Research agents. We begin by reviewing information acquisition strategies, contrasting API-based retrieval methods with browser-based exploration. We then examine modular tool-use frameworks, including code execution, multimodal input processing, and the integration of Model Context Protocols (MCPs) to support extensibility and ecosystem development. To systematize existing approaches, we propose a taxonomy that differentiates between static and dynamic workflows, and we classify agent architectures based on planning strategies and agent composition, including single-agent and multi-agent configurations. We also provide a critical evaluation of current benchmarks, highlighting key limitations such as restricted access to external knowledge, sequential execution inefficiencies, and misalignment between evaluation metrics and the practical objectives of DR agents. Finally, we outline open challenges and promising directions for future research. A curated and continuously updated repository of DR agent research is available at: {https://github.com/ai-agents-2030/awesome-deep-research-agent}.

## From the paper (full-text excerpts)
**Introduction.** Introduction Contribution. Survey Organization. 2 Background and Preliminaries 2.1 Advances in Reasoning and Tool Integration 2.2 Advances in Retrieval-Augmented Generation and Agentic Retrieval 2.3 Model Context Protocol and Agent-to-Agent Policy 3 Deep Research: Search Engine, Tool Use, Workflow, Tuning, Non-parametric Continual Learning 3.1 Search Engine: API vs. Browser 3.2 Tool Use: Empowering Agents with Extended Functionalities Code Interpreter. Data Analytics. Multimodal Processing and Generation. Deep Research Agent with Computer Use. 3.3 Architecture and Workflow 3.3.1 Static vs. Dynamic Workflows Static Workflows. Dynamic Workflows. 3.3.2 Dynamic Workflows: Planning Strategies 3.3.3 Dynamic Workflows: Single-Agent vs. Multi-Agent Dynamic Single-Agent Systems. Dynamic Multi-Agent Systems. 3.3.4 Memory Mechanism for Long-Context Optimisation 3.4 Tuning: Beyond Prompting toward Capability Enhancement Parametric Approaches. 3.4.1 SFT-based Optimization 3.4.2 Reinforcement Learning-based Optimisation…

**Method / approach.** methods with browser-based exploration. We then examine modular tool-use frameworks, including code execution, multimodal input processing, and the integration of Model Context Protocols (MCPs) to support extensibility and ecosystem development. To systematise existing approaches, we propose a taxonomy that differentiates between static and dynamic workflows, and we classify agent architectures based on planning strategies and agent composition, including single-agent and multi-agent configurations. We also provide a critical evaluation of current benchmarks, highlighting key limitations such as restricted access to external knowledge, sequential execution inefficiencies, and misalignment between evaluation metrics and the practical objectives of DR agents. Finally, we outline open challenges and promising directions for future research. A curated and continuously updated repository of DR agent research is available at: https://github.com/ai-agents-2030/awesome-deep-research-agent .…

**Results.** experiment execution, and structured drafting through tool-augmented research pipelines. Towards an AI co-scientist and O-agents ( gottweis2025towards, ; zhu2025oagents, ) outline blueprints and empirical recipes for building, training, and evaluating effective tool-using research agents. Agent-KB ( tang2025agent, ) introduces a KB-driven framework for cross-domain experience transfer to boost generalisation on complex tasks. Microsoft Copilot Researcher ( microsoft_copilot_researcher, ) embeds multi-step research and analytics in the Microsoft 365 ecosystem, producing reports and charts within enterprise workflows. Alita ( qiu2025alita, ) explores self-evolving agents that generate and wrap MCP tools, alongside code execution, to extend capabilities with minimal predefined schemas. 3.3 Architecture and Workflow As shown in Figure 4 , this section systematically analyses the construction of DR systems, focusing on workflows c…

**Conclusion.** Conclusion Deep Research Agents: A Systematic Examination And Roadmap Yuxuan Huang † Yihang Chen † Haozheng Zhang † Kang Li Huichi Zhou Meng Fang Linyi Yang Xiaoguang Li Lifeng Shang Songcen Xu Jianye Hao Kun Shao ‡ Jun Wang ‡ Abstract The rapid progress of Large Language Models (LLMs) has given rise to a new category of autonomous AI systems, referred to as Deep Research (DR) agents. These agents are designed to tackle complex, multi-turn informational research tasks by leveraging a combination of dynamic reasoning, adaptive long-horizon planning, multi-hop information retrieval, iterative tool use, and the generation of structured analytical reports. In this paper, we conduct a detailed analysis of…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[science-agents|Science agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2506.18096v2.md` · `raw/arxiv/2506.18096v2.fulltext.md`
