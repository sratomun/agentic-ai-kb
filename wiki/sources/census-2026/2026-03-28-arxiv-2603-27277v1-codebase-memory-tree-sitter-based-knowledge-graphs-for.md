---
type: source
source_type: arxiv
title: "Codebase-Memory: Tree-Sitter-Based Knowledge Graphs for LLM Code Exploration via MCP"
authors: Martin Vogel, Falk Meyer-Eschenbach, Severin Kohler, Elias Grünewald et al.
url: https://arxiv.org/abs/2603.27277v1
date: 2026-03-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.SE
tags: [coding-agents, knowledge-graph, agent-protocols, agent-memory, tool-use, arxiv, auto-ingested]
---

# Codebase-Memory: Tree-Sitter-Based Knowledge Graphs for LLM Code Exploration via MCP

**arXiv:** [2603.27277v1](https://arxiv.org/abs/2603.27277v1) · 2026-03-28 · cs.SE
**Authors:** Martin Vogel, Falk Meyer-Eschenbach, Severin Kohler, Elias Grünewald et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) coding agents typically explore codebases through repeated file-reading and grep-searching, consuming thousands of tokens per query without structural understanding. We present Codebase-Memory, an open-source system that constructs a persistent, Tree-Sitter-based knowledge graph via the Model Context Protocol (MCP), parsing 66 languages through a multi-phase pipeline with parallel worker pools, call-graph traversal, impact analysis, and community discovery. Evaluated across 31 real-world repositories, Codebase-Memory achieves 83% answer quality versus 92% for a file-exploration agent, at ten times fewer tokens and 2.1 times fewer tool calls. For graph-native queries such as hub detection and caller ranking, it matches or exceeds the explorer on 19 of 31 languages.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.27277v1)
