---
type: source
source_type: arxiv
title: "Benchmarking Text-to-Python against Text-to-SQL: The Impact of Explicit Logic and Ambiguity"
authors: Hangle Hu, Chenyu Hou, Bin Cao, Ruizhe Li
url: https://arxiv.org/abs/2601.15728v2
date: 2026-01-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.AI
tags: [data-query-agents, coding-agents, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# Benchmarking Text-to-Python against Text-to-SQL: The Impact of Explicit Logic and Ambiguity

**arXiv:** [2601.15728v2](https://arxiv.org/abs/2601.15728v2) · 2026-01-22 · cs.AI
**Authors:** Hangle Hu, Chenyu Hou, Bin Cao, Ruizhe Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Text-to-SQL remains the dominant approach for database interaction, real-world analytics increasingly require the flexibility of general-purpose programming languages such as Python or Pandas to manage file-based data and complex analytical workflows. Despite this growing need, the reliability of Text-to-Python in core data retrieval remains underexplored relative to the mature SQL ecosystem. To address this gap, we introduce BIRD-Python, a benchmark designed for cross-paradigm evaluation. We systematically refined the original dataset to reduce annotation noise and align execution semantics, thereby establishing a consistent and standardized baseline for comparison. Our analysis reveals a fundamental paradigmatic divergence: whereas SQL leverages implicit DBMS behaviors through its declarative structure, Python requires explicit procedural logic, making it highly sensitive to underspecified user intent. To mitigate this challenge, we propose the Logic Completion Framework (LCF), which resolves ambiguity by incorporating latent domain knowledge into the generation process. Experimental results show that (1) performance differences primarily stem from missing domain context rather than inherent limitations in code generation, and (2) when these gaps are addressed, Text-to-Python achieves performance parity with Text-to-SQL. These findings establish Python as a viable foundation for analytical agents-provided that systems effectively ground ambiguous natural language inputs in executable logical specifications. Resources are available at https://anonymous.4open.science/r/Bird-Python-43B7/.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.15728v2)
