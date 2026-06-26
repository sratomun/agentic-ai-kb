---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks via MCP Servers"
authors: Zhenting Wang, Qi Chang, Hemani Patel, Shashank Biju et al.
url: https://arxiv.org/abs/2508.20453v1
date: 2025-08-28
citationCount: 74
influentialCitationCount: 6
velocity: 7.56
ingested: 2026-06-22
tags: [finance-agents, agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, 2025, cited]
---

# MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks via MCP Servers

**arXiv [2508.20453v1](https://arxiv.org/abs/2508.20453v1)** · 2025-08-28 · **74 citations** (6 influential · 7.56/mo) · Zhenting Wang, Qi Chang, Hemani Patel, Shashank Biju et al.

## Abstract
We introduce MCP-Bench, a benchmark for evaluating large language models (LLMs) on realistic, multi-step tasks that demand tool use, cross-tool coordination, precise parameter control, and planning/reasoning for solving tasks. Built on the Model Context Protocol (MCP), MCP-Bench connects LLMs to 28 representative live MCP servers spanning 250 tools across domains such as finance, traveling, scientific computing, and academic search. Unlike prior API-based benchmarks, each MCP server provides a set of complementary tools designed to work together, enabling the construction of authentic, multi-step tasks with rich input-output coupling. Tasks in MCP-Bench test agents' ability to retrieve relevant tools from fuzzy instructions without explicit tool names, plan multi-hop execution trajectories for complex objectives, ground responses in intermediate tool outputs, and orchestrate cross-domain workflows - capabilities not adequately evaluated by existing benchmarks that rely on explicit tool specifications, shallow few-step workflows, and isolated domain operations. We propose a multi-faceted evaluation framework covering tool-level schema understanding and usage, trajectory-level planning, and task completion. Experiments on 20 advanced LLMs reveal persistent challenges in MCP-Bench. Code and data: https://github.com/Accenture/mcp-bench.

## From the paper (full-text excerpts)
**Introduction.** Introduction Recent advances in large language models (LLMs) have enabled a new generation of tool-using agents that can interpret natural language instructions, plan multi-step workflows, and interact with external tools to solve complex tasks (OpenAI, 2025c; Comanici et al., 2025; Anthropic, 2025; Yang et al., 2025; Kimi et al., 2025; Zeng et al., 2025; Chen et al., 2025). Such agents are increasingly deployed in real-world domains such as travel (Xie et al., 2024), healthcare (Saab et al., 2024; Mehandru et al., 2024), and finance (Xiao et al., 2024), where solving user queries requires chaining multiple tools, reasoning over structured outputs, and coordinating interdependent operations. Despite rapid progress in LLM agents, existing benchmarks for tool use remain fundamentally limited. Early efforts such as ToolBench (Qin et al., 2024) and BFCL v3 (Patil et al., 2025a) aggregate large collections of APIs, but these APIs are designed for isolated functionality. As a result, tasks often reduce to few-step tool calls or rely on artificially stitched pipelines, since tool inputs and…

**Method / approach.** Method and Metrics We use a comprehensive evaluation framework combining rule-based metrics and LLM judge scoring. The rule-based component measures tool usage robustness across four dimensions—name validity, schema adherence, runtime success, and dependency compliance—from execution traces. The LLM-as-a- 7 MCP-Bench: Benchmarking Tool-Using LLM Agents with Complex Real-World Tasks via MCP Servers Judge component assesses strategic quality in task completion, tool selection, and planning efficiency and effectiveness, using structured rubrics with prompt shuffling and score averaging to ensure fairness. 5.1. Rule-based Evaluation To assess the schema understanding and execution robustness of an agent’s behavior, we evaluate its tool usage along dimensions of name validity, input schema adherence, and runtime success. Let 𝐸 = { 𝑒1 , . . . , 𝑒𝑘 } be the set of all tool invocations during execution. Tool Name Validity Rate. This metric assesses whether the agent selects tools that exi…

**Results.** Experiments on 20 advanced LLMs reveal persistent challenges in M C P- Be nc h. Code and data: https://github.com/Accenture/mcp-bench. 1. Introduction Recent advances in large language models (LLMs) have enabled a new generation of tool-using agents that can interpret natural language instructions, plan multi-step workflows, and interact with external tools to solve complex tasks (OpenAI, 2025c; Comanici et al., 2025; Anthropic, 2025; Yang et al., 2025; Kimi et al., 2025; Zeng et al., 2025; Chen et al., 2025). Such agents are increasingly deployed in real-world domains such as travel (Xie et al., 2024), healthcare (Saab et al., 2024; Mehandru et al., 2024), and finance (Xiao et al., 2024), where solving user queries requires chaining multiple tools, reasoning over structured outputs, and coordinating interdependent operations. Despite rapid progress in LLM agents, existing benchmarks for tool use remain fundamentally limited. Early eff…

**Conclusion.** Conclusion In this paper, we introduced M C P- Be nc h, a large-scale benchmark for evaluating LLM agents in realistic, ecosystem-based tool-use scenarios. Built on MCP, M C P- Be nc h connects agents to 28 production servers with 250 tools, enabling complex multi-hop workflows and cross-domain orchestration. Our automated task synthesis pipeline generates 104 challenging tasks with fuzzy instructions that require strong agentic capabilities to solve. Through our evaluation framework combining rule-based checks and LLM Judge scoring, we revealed that even state-of-the-art models struggle with different capabilities such as dependency chain compliance, tool selection under noisy environment, and long-horizon planning. 13 MCP-Bench: Benchm…

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Raw:** `raw/arxiv/2508.20453v1.md` · `raw/arxiv/2508.20453v1.fulltext.md`
