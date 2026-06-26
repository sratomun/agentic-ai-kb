---
type: source
source_type: arxiv
title: "Evaluating Temporal Semantic Caching and Workflow Optimization in Agentic Plan-Execute Pipelines"
authors: Alimurtaza Mustafa Merchant, Krish Veera, Sajal Kumar Goyla, Shambhawi Bhure et al.
url: https://arxiv.org/abs/2605.20630v1
date: 2026-05-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Evaluating Temporal Semantic Caching and Workflow Optimization in Agentic Plan-Execute Pipelines

**arXiv:** [2605.20630v1](https://arxiv.org/abs/2605.20630v1) · 2026-05-20 · cs.AI
**Authors:** Alimurtaza Mustafa Merchant, Krish Veera, Sajal Kumar Goyla, Shambhawi Bhure et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Industrial asset operations workflows are latency-sensitive because a single user query may require coordination over sensor data, work orders, failure modes, forecasting tools, and domain-specific agents. We evaluate this problem on AssetOpsBench (AOB), an industrial agent benchmark whose plan-execute pipeline exposes repeated overhead from tool discovery, LLM planning, MCP tool execution, and final summarization. Existing LLM caching techniques such as KV-cache reuse and embedding-based semantic caching were designed for chatbot serving and break down when output validity depends on time, asset, or sensor parameters. We propose two complementary optimization layers for AOB plan-execute pipelines: a temporal semantic cache and a set of MCP workflow optimizations combining disk-backed tool-discovery caching and dependency-aware parallel step execution. MCP workflow optimizations corresponded to a 1.67x speedup and reduced median end-to-end latency by about 40.0% while the temporal-cache benchmark achieved a median of 30.6x speedup on cache hits. Beyond the speedup, our results expose a concrete failure mode of pure semantic caching for parameter-rich industrial queries, providing a critical analysis of how caching choices interact with evaluation correctness in MCP-backed agent benchmarks.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.20630v1)
