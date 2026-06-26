---
type: source
source_type: arxiv
title: "Semantic Tool Discovery for Large Language Models: A Vector-Based Approach to MCP Tool Selection"
authors: Sarat Mudunuri, Jian Wan, Ally Qin, Srinivasan Manoharan
url: https://arxiv.org/abs/2603.20313v1
date: 2026-03-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.SE
tags: [agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Semantic Tool Discovery for Large Language Models: A Vector-Based Approach to MCP Tool Selection

**arXiv:** [2603.20313v1](https://arxiv.org/abs/2603.20313v1) · 2026-03-19 · cs.SE
**Authors:** Sarat Mudunuri, Jian Wan, Ally Qin, Srinivasan Manoharan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) with tool-calling capabilities have demonstrated remarkable potential in executing complex tasks through external tool integration. The Model Context Protocol (MCP) has emerged as a standardized framework for connecting LLMs to diverse toolsets, with individual MCP servers potentially exposing dozens to hundreds of tools. However, current implementations face a critical scalability challenge: providing all available tools to the LLM context results in substantial token overhead, increased costs, reduced accuracy, and context window constraints. We present a semantic tool discovery architecture that addresses these challenges through vector-based retrieval. Our approach indexes MCP tools using dense embeddings that capture semantic relationships between tool capabilities and user intent, dynamically selecting only the most relevant tools (typically 3-5) rather than exposing the entire tool catalog (50-100+). Experimental results demonstrate a 99.6% reduction in tool-related token consumption with a hit rate of 97.1% at K=3 and an MRR of 0.91 on a benchmark of 140 queries across 121 tools from 5 MCP servers, with sub-100ms retrieval latency. Contributions include: (1) a semantic indexing framework for MCP tools, (2) a dynamic tool selection algorithm based on query-tool similarity, (3) comprehensive evaluation demonstrating significant efficiency and accuracy improvements, and (4) extensibility to multi-agent and cross-organizational tool discovery.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.20313v1)
