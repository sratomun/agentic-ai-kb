---
type: source
source_type: arxiv
title: "An Agentic Evaluation Framework for AI-Generated Scientific Code in PETSc"
authors: Hong Zhang, Barry Smith, Satish Balay, Le Chen et al.
url: https://arxiv.org/abs/2603.15976v1
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [coding-agents, agent-protocols, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# An Agentic Evaluation Framework for AI-Generated Scientific Code in PETSc

**arXiv:** [2603.15976v1](https://arxiv.org/abs/2603.15976v1) · 2026-03-16 · cs.AI
**Authors:** Hong Zhang, Barry Smith, Satish Balay, Le Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While large language models have significantly accelerated scientific code generation, comprehensively evaluating the generated code remains a major challenge. Traditional benchmarks reduce evaluation to test-case matching, an approach insufficient for library code in HPC where solver selection, API conventions, memory management, and performance are just as critical as functional correctness. To address this gap, we introduce petscagent-bench, an agentic framework built on an agents-evaluating-agents paradigm. Instead of relying on static scripts, petscagent-bench deploys a tool-augmented evaluator agent that compiles, executes, and measures code produced by a separate model-under-test agent, orchestrating a 14-evaluator pipeline across five scoring categories: correctness, performance, code quality, algorithmic appropriateness, and library-specific conventions. Because the agents communicate through standardized protocols (A2A and MCP), the framework enables black-box evaluation of any coding agent without requiring access to its source code. We demonstrate the framework on a benchmark suite of realistic problems using the PETSc library for HPC. Our empirical analysis of frontier models reveals that while current models generate readable, well-structured code, they consistently struggle with library-specific conventions that traditional pass/fail metrics completely miss.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[a2a-protocol]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.15976v1)
