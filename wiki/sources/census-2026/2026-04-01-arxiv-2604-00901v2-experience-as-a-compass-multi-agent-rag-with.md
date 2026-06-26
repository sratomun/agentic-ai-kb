---
type: source
source_type: arxiv
title: "Experience as a Compass: Multi-agent RAG with Evolving Orchestration and Agent Prompts"
authors: Sha Li, Naren Ramakrishnan
url: https://arxiv.org/abs/2604.00901v2
date: 2026-04-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agentic-rl, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Experience as a Compass: Multi-agent RAG with Evolving Orchestration and Agent Prompts

**arXiv:** [2604.00901v2](https://arxiv.org/abs/2604.00901v2) · 2026-04-01 · cs.AI
**Authors:** Sha Li, Naren Ramakrishnan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent Retrieval-Augmented Generation (RAG), wherein each agent takes on a specific role, supports hard queries that require multiple steps and sources, or complex reasoning. Existing approaches, however, rely on static agent behaviors and fixed orchestration strategies, leading to brittle performance on diverse, multi-hop tasks. We identify two key limitations: the lack of continuously adaptive orchestration mechanisms and the absence of behavior-level learning for individual agents. To this end, we propose HERA, a hierarchical framework that jointly evolves multi-agent orchestration and role-specific agent prompts. At the global level, HERA optimizes query-specific agent topologies through reward-guided sampling and experience accumulation. At the local level, Role-Aware Prompt Evolution refines agent behaviors via credit assignment and dual-axes adaptation along operational and behavioral principles, enabling targeted, role-conditioned improvements. On six knowledge-intensive benchmarks, HERA achieves an average improvement of 38.69\% over recent baselines while maintaining robust generalization and token efficiency. Topological analyses reveal emergent self-organization, where sparse exploration yields compact, high-utility multi-agent networks, demonstrating both efficient coordination and robust reasoning.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.00901v2)
