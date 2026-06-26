---
type: source
source_type: arxiv
title: "Agentic Diagnostic Reasoning over Telecom and Datacenter Infrastructure"
authors: Nicolas Tacheny
url: https://arxiv.org/abs/2601.07342v1
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, agent-protocols, arxiv, auto-ingested]
---

# Agentic Diagnostic Reasoning over Telecom and Datacenter Infrastructure

**arXiv:** [2601.07342v1](https://arxiv.org/abs/2601.07342v1) · 2026-01-12 · cs.AI
**Authors:** Nicolas Tacheny

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large-scale telecom and datacenter infrastructures rely on multi-layered service and resource models, where failures propagate across physical and logical components and affect multiple customers. Traditional approaches to root cause analysis(RCA) rely on hard-coded graph traversal algorithms or rule-based correlation engines, which are costly to maintain and tightly coupled to the infrastructure model. In this work, we introduce an agentic diagnostic framework where a Large Language Model (LLM) performs step-wise investigation using a constrained tool space exposed through the Model Context Protocol (MCP). Instead of embedding causal logic or traversal algorithms into the application, the agent autonomously navigates the infrastructure model by invoking tools for service lookup, dependency retrieval, structured and unstructured data, and event analysis, and impact discovery. We define an investigation protocol that structures the agent's reasoning and ensures grounding, reproducibility, and safe handling of missing or ambiguous information. This work lays the foundation for autonomous incident resolution and change impact mitigation. Future systems will not only diagnose and remediate infrastructure failures, but also predict the impact of planned changes on services and customers, enabling operators to mitigate risks before executing maintenance operations.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-protocols|Agent protocols]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.07342v1)
