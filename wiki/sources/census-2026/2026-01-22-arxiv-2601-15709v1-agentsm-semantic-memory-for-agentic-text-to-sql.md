---
type: source
source_type: arxiv
title: "AgentSM: Semantic Memory for Agentic Text-to-SQL"
authors: Asim Biswal, Chuan Lei, Xiao Qin, Aodong Li et al.
url: https://arxiv.org/abs/2601.15709v1
date: 2026-01-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [data-query-agents, agent-reliability, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# AgentSM: Semantic Memory for Agentic Text-to-SQL

**arXiv:** [2601.15709v1](https://arxiv.org/abs/2601.15709v1) · 2026-01-22 · cs.AI
**Authors:** Asim Biswal, Chuan Lei, Xiao Qin, Aodong Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in LLM-based Text-to-SQL have achieved remarkable gains on public benchmarks such as BIRD and Spider. Yet, these systems struggle to scale in realistic enterprise settings with large, complex schemas, diverse SQL dialects, and expensive multi-step reasoning. Emerging agentic approaches show potential for adaptive reasoning but often suffer from inefficiency and instability-repeating interactions with databases, producing inconsistent outputs, and occasionally failing to generate valid answers. To address these challenges, we introduce Agent Semantic Memory (AgentSM), an agentic framework for Text-to-SQL that builds and leverages interpretable semantic memory. Instead of relying on raw scratchpads or vector retrieval, AgentSM captures prior execution traces-or synthesizes curated ones-as structured programs that directly guide future reasoning. This design enables systematic reuse of reasoning paths, which allows agents to scale to larger schemas, more complex questions, and longer trajectories efficiently and reliably. Compared to state-of-the-art systems, AgentSM achieves higher efficiency by reducing average token usage and trajectory length by 25% and 35%, respectively, on the Spider 2.0 benchmark. It also improves execution accuracy, reaching a state-of-the-art accuracy of 44.8% on the Spider 2.0 Lite benchmark.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]] · [[spider-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.15709v1)
