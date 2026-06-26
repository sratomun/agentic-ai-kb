---
type: source
source_type: arxiv
title: "STEM Agent: A Self-Adapting, Tool-Enabled, Extensible Architecture for Multi-Protocol AI Agent Systems"
authors: Alfred Shen, Aaron Shen
url: https://arxiv.org/abs/2603.22359v1
date: 2026-03-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-protocols, agent-skills, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# STEM Agent: A Self-Adapting, Tool-Enabled, Extensible Architecture for Multi-Protocol AI Agent Systems

**arXiv:** [2603.22359v1](https://arxiv.org/abs/2603.22359v1) · 2026-03-22 · cs.AI
**Authors:** Alfred Shen, Aaron Shen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current AI agent frameworks commit early to a single interaction protocol, a fixed tool integration strategy, and static user models, limiting their deployment across diverse interaction paradigms. To address these constraints, we introduce STEM Agent (Self-adapting, Tool-enabled, Extensible, Multi-agent), a modular architecture inspired by biological pluripotency in which an undifferentiated agent core differentiates into specialized protocol handlers, tool bindings, and memory subsystems that compose into a fully functioning AI system. The framework unifies five interoperability protocols (A2A, AG-UI, A2UI, UCP, and AP2) behind a single gateway, introduces a Caller Profiler that continuously learns user preferences across more than twenty behavioral dimensions, externalizes all domain capabilities through the Model Context Protocol (MCP), and implements a biologically inspired skills acquisition system in which recurring interaction patterns crystallize into reusable agent skills through a maturation lifecycle analogous to cell differentiation. Complementing these capabilities, the memory system incorporates consolidation mechanisms, including episodic pruning, semantic deduplication, and pattern extraction, designed for sub-linear growth under sustained interaction. A comprehensive 413-test suite validates protocol handler behavior and component integration across all five architectural layers, completing in under three seconds.

## Graph
- **Concepts:** [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]] · [[a2a-protocol]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.22359v1)
