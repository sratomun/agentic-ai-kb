---
type: source
source_type: arxiv
title: "Autogenesis: A Self-Evolving Agent Protocol"
authors: Wentao Zhang, Zhe Zhao, Haibin Wen, Yingcheng Wu et al.
url: https://arxiv.org/abs/2604.15034v4
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [self-evolving-agents, agent-protocols, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Autogenesis: A Self-Evolving Agent Protocol

**arXiv:** [2604.15034v4](https://arxiv.org/abs/2604.15034v4) · 2026-04-16 · cs.AI
**Authors:** Wentao Zhang, Zhe Zhao, Haibin Wen, Yingcheng Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in LLM based agent systems have shown promise in tackling complex, long horizon tasks. However, existing agent protocols (e.g., A2A and MCP) under specify cross entity lifecycle and context management, version tracking, and evolution safe update interfaces, which encourages monolithic compositions and brittle glue code. We introduce Autogenesis Protocol (AGP), a self evolution protocol that decouples what evolves from how evolution occurs. Its Resource Substrate Protocol Layer (RSPL) models prompts, agents, tools, environments, and memory as protocol registered resources with explicit state, lifecycle, and versioned interfaces. Its Self Evolution Protocol Layer (SEPL) specifies a closed loop operator interface for proposing, assessing, and committing improvements with auditable lineage and rollback. Building on AGP, we present Autogenesis System (AGS), a self-evolving multi-agent system that dynamically instantiates, retrieves, and refines protocol-registered resources during execution. We evaluate AGS on multiple challenging benchmarks that require long horizon planning and tool use across heterogeneous resources. The results demonstrate consistent improvements over strong baselines, supporting the effectiveness of agent resource management and closed loop self evolution. The code is available at https://github.com/DVampire/Autogenesis.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]] · [[a2a-protocol]] · [[autogen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.15034v4)
