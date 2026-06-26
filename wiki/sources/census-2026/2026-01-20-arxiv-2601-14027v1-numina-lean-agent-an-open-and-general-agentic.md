---
type: source
source_type: arxiv
title: "Numina-Lean-Agent: An Open and General Agentic Reasoning System for Formal Mathematics"
authors: Junqi Liu, Zihao Zhou, Zekai Zhu, Marco Dos Santos et al.
url: https://arxiv.org/abs/2601.14027v1
date: 2026-01-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [coding-agents, agent-protocols, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Numina-Lean-Agent: An Open and General Agentic Reasoning System for Formal Mathematics

**arXiv:** [2601.14027v1](https://arxiv.org/abs/2601.14027v1) · 2026-01-20 · cs.AI
**Authors:** Junqi Liu, Zihao Zhou, Zekai Zhu, Marco Dos Santos et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic systems have recently become the dominant paradigm for formal theorem proving, achieving strong performance by coordinating multiple models and tools. However, existing approaches often rely on task-specific pipelines and trained formal provers, limiting their flexibility and reproducibility. In this paper, we propose the paradigm that directly uses a general coding agent as a formal math reasoner. This paradigm is motivated by (1) A general coding agent provides a natural interface for diverse reasoning tasks beyond proving, (2) Performance can be improved by simply replacing the underlying base model, without training, and (3) MCP enables flexible extension and autonomous calling of specialized tools, avoiding complex design. Based on this paradigm, we introduce Numina-Lean-Agent, which combines Claude Code with Numina-Lean-MCP to enable autonomous interaction with Lean, retrieval of relevant theorems, informal proving and auxiliary reasoning tools. Using Claude Opus 4.5 as the base model, Numina-Lean-Agent solves all problems in Putnam 2025 (12 / 12), matching the best closed-source system. Beyond benchmark evaluation, we further demonstrate its generality by interacting with mathematicians to successfully formalize the Brascamp-Lieb theorem. We release Numina-Lean-Agent and all solutions at https://github.com/project-numina/numina-lean-agent.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.14027v1)
