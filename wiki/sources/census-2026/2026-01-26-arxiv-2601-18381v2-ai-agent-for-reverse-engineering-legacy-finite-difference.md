---
type: source
source_type: arxiv
title: "AI Agent for Reverse-Engineering Legacy Finite-Difference Code and Translating to Devito"
authors: Yinghan Hou, Zongyou Yang
url: https://arxiv.org/abs/2601.18381v2
date: 2026-01-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [knowledge-graph, agent-reliability, agentic-rl, agentic-rag, governance-gap, arxiv, auto-ingested]
---

# AI Agent for Reverse-Engineering Legacy Finite-Difference Code and Translating to Devito

**arXiv:** [2601.18381v2](https://arxiv.org/abs/2601.18381v2) · 2026-01-26 · cs.AI
**Authors:** Yinghan Hou, Zongyou Yang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
To facilitate the transformation of legacy finite difference implementations into the Devito environment, this study develops an integrated AI agent framework. Retrieval-Augmented Generation (RAG) and open-source Large Language Models are combined through multi-stage iterative workflows in the system's hybrid LangGraph architecture. The agent constructs an extensive Devito knowledge graph through document parsing, structure-aware segmentation, extraction of entity relationships, and Leiden-based community detection. GraphRAG optimisation enhances query performance across semantic communities that include seismic wave simulation, computational fluid dynamics, and performance tuning libraries. A reverse engineering component derives three-level query strategies for RAG retrieval through static analysis of Fortran source code. To deliver precise contextual information for language model guidance, the multi-stage retrieval pipeline performs parallel searching, concept expansion, community-scale retrieval, and semantic similarity analysis. Code synthesis is governed by Pydantic-based constraints to guarantee structured outputs and reliability. A comprehensive validation framework integrates conventional static analysis with the G-Eval approach, covering execution correctness, structural soundness, mathematical consistency, and API compliance. The overall agent workflow is implemented on the LangGraph framework and adopts concurrent processing to support quality-based iterative refinement and state-aware dynamic routing. The principal contribution lies in the incorporation of feedback mechanisms motivated by reinforcement learning, enabling a transition from static code translation toward dynamic and adaptive analytical behavior.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[governance-gap|Governance gap]]
- **Entities:** [[graphrag]] · [[langgraph]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.18381v2)
