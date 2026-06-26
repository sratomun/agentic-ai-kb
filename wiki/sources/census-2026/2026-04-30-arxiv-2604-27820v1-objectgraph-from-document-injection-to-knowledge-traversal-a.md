---
type: source
source_type: arxiv
title: "ObjectGraph: From Document Injection to Knowledge Traversal -- A Native File Format for the Agentic Era"
authors: Mohit Dubey, Open Gigantic
url: https://arxiv.org/abs/2604.27820v1
date: 2026-04-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [knowledge-graph, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# ObjectGraph: From Document Injection to Knowledge Traversal -- A Native File Format for the Agentic Era

**arXiv:** [2604.27820v1](https://arxiv.org/abs/2604.27820v1) · 2026-04-30 · cs.AI
**Authors:** Mohit Dubey, Open Gigantic

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Every document format in existence was designed for a human reader moving linearly through text. Autonomous LLM agents do not read - they retrieve. This fundamental mismatch forces agents to inject entire documents into their context window, wasting tokens on irrelevant content, compounding state across multi-turn loops, and broadcasting information indiscriminately across agent roles. We argue this is not a prompt engineering problem, not a retrieval problem, and not a compression problem: it is a format problem. We introduce OBJECTGRAPH (.og), a file format that reconceives the document as a typed, directed knowledge graph to be traversed rather than a string to be injected. OBJECTGRAPH is a strict superset of Markdown - every .md file is a valid .og file - requires no infrastructure beyond a two-primitive query protocol, and is readable by both humans and agents without tooling. We formalize the Document Consumption Problem, characterise six structural properties no existing format satisfies simultaneously, and prove OBJECTGRAPH satisfies all six. We further introduce the Progressive Disclosure Model, the Role-Scoped Access Protocol, and Executable Assertion Nodes as native format primitives. Empirical evaluation across five document classes and eight agent task types demonstrates up to 95.3 percent token reduction with no statistically significant degradation in task accuracy (p > 0.05). Transpiler fidelity reaches 98.7 percent content preservation on a held-out document benchmark.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.27820v1)
