---
type: source
source_type: arxiv
title: "Towards Agentic Test-Driven Quality Assurance for 6G Networks"
authors: Christos Tranoris, Besiana Agko, Kostis Trantzas, Irene Denazi
url: https://arxiv.org/abs/2604.23285v1
date: 2026-04-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 28
primary: cs.NI
tags: [coding-agents, agent-reliability, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Towards Agentic Test-Driven Quality Assurance for 6G Networks

**arXiv:** [2604.23285v1](https://arxiv.org/abs/2604.23285v1) · 2026-04-25 · cs.NI
**Authors:** Christos Tranoris, Besiana Agko, Kostis Trantzas, Irene Denazi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This work proposes an agentic, intent-driven end-to-end (E2E) orchestration framework that integrates intent co-creation with a Test-Driven Quality Assurance paradigm. In this framework, autonomous agents iteratively refine a user's initial intent into a confirmed, auditable specification. Furthermore, the system automatically derives validation tests from these intents before provisioning, directly mirroring the Test-Driven Development workflow in software engineering to ensure proactive Service Level Agreement (SLA) compliance. The architecture is grounded in a standards-aligned knowledge representation using TM Forum (TMF) information models and catalogs. This enables deterministic graph traversal from high-level Product Offerings down to granular Service/Resource and Test specifications. We prototyped this architecture by extending OpenSlice with a message-driven, multi-agent pattern and integrating MCP-enabled (Model Context Protocol) tool access for real-time knowledge retrieval. Currently, our evaluation of the agents targets the intent co-creation phase as a baseline toward full-scale orchestration. Building on experiments with multiple open-source Large Language Model (LLM) backends integrated with the TMF-based knowledge base, we observe substantial variability in tool-use reliability and hallucination patterns, underscoring the critical importance of robust knowledge integration in agentic 6G systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23285v1)
