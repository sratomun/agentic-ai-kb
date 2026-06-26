---
type: source
source_type: arxiv
title: "From Tool Orchestration to Code Execution: A Study of MCP Design Choices"
authors: Yuval Felendler, Parth A. Gandhi, Idan Habler, Yuval Elovici et al.
url: https://arxiv.org/abs/2602.15945v1
date: 2026-02-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CR
tags: [agent-security, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# From Tool Orchestration to Code Execution: A Study of MCP Design Choices

**arXiv:** [2602.15945v1](https://arxiv.org/abs/2602.15945v1) · 2026-02-17 · cs.CR
**Authors:** Yuval Felendler, Parth A. Gandhi, Idan Habler, Yuval Elovici et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Model Context Protocols (MCPs) provide a unified platform for agent systems to discover, select, and orchestrate tools across heterogeneous execution environments. As MCP-based systems scale to incorporate larger tool catalogs and multiple concurrently connected MCP servers, traditional tool-by-tool invocation increases coordination overhead, fragments state management, and limits support for wide-context operations. To address these scalability challenges, recent MCP designs have incorporated code execution as a first-class capability, an approach called Code Execution MCP (CE-MCP). This enables agents to consolidate complex workflows, such as SQL querying, file analysis, and multi-step data transformations, into a single program that executes within an isolated runtime environment. In this work, we formalize the architectural distinction between context-coupled (traditional) and context-decoupled (CE-MCP) models, analyzing their fundamental scalability trade-offs. Using the MCP-Bench framework across 10 representative servers, we empirically evaluate task behavior, tool utilization patterns, execution latency, and protocol efficiency as the scale of connected MCP servers and available tools increases, demonstrating that while CE-MCP significantly reduces token usage and execution latency, it introduces a vastly expanded attack surface. We address this security gap by applying the MAESTRO framework, identifying sixteen attack classes across five execution phases-including specific code execution threats such as exception-mediated code injection and unsafe capability synthesis. We validate these vulnerabilities through adversarial scenarios across multiple LLMs and propose a layered defense architecture comprising containerized sandboxing and semantic gating. Our findings provide a rigorous roadmap for balancing scalability and security in production-ready executable agent workflows.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.15945v1)
