---
type: source
source_type: arxiv
kind: survey
title: "Inside the Scaffold: A Source-Code Taxonomy of Coding Agent Architectures"
authors: Benjamin Rombaut
url: https://arxiv.org/abs/2604.03515v2
date: 2026-04-03
ingested: 2026-06-21
depth: full-text
tags: [coding-agents, tool-use, multi-agent-systems, arxiv, survey]
---

# Inside the Scaffold: A Source-Code Taxonomy of Coding Agent Architectures

**SURVEY** · arXiv [2604.03515v2](https://arxiv.org/abs/2604.03515v2) · 2026-04-03 · Benjamin Rombaut

**Why it matters:** The most concrete look at how real coding agents are actually built — useful when evaluating or designing agent scaffolds.

## What it surveys
Coding-agent *scaffolds* — the control loop, tool definitions, state management, and context strategy around the model — from source-code analysis of 13 open-source agents at pinned commits.

## Framework / taxonomy
A source-code-level taxonomy across 12 dimensions in three layers (control architecture, tool/environment interface, resource management); identifies five composable loop primitives: ReAct, generate-test-repair, plan-execute, multi-attempt retry, tree search.

## Notable points
- 11 of 13 agents compose multiple loop primitives rather than using one control structure.
- Wide divergence in context-compaction (7 strategies) and tool counts (0–37); convergence where external constraints dominate.
- Every taxonomic claim grounded in file paths/line numbers — a reusable engineering reference.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Raw:** `raw/arxiv/2604.03515v2.md` · `raw/arxiv/2604.03515v2.fulltext.md`

