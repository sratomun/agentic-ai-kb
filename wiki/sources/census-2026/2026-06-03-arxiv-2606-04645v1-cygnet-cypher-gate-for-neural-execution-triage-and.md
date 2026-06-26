---
type: source
source_type: arxiv
title: "CYGNET: Cypher Gate for Neural Execution Triage and Cost Containment"
authors: Nikodem Tomczak
url: https://arxiv.org/abs/2606.04645v1
date: 2026-06-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 0
primary: cs.CL
tags: [knowledge-graph, arxiv, auto-ingested]
---

# CYGNET: Cypher Gate for Neural Execution Triage and Cost Containment

**arXiv:** [2606.04645v1](https://arxiv.org/abs/2606.04645v1) · 2026-06-03 · cs.CL
**Authors:** Nikodem Tomczak

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Language models acting as agents over knowledge graphs generate Cypher queries that fail structurally (crashing at the database) or semantically (executing but returning wrong results). We place a pre-execution gate between query generation and a production Neo4j database. The gate validates structure through a four-backend chain culminating in execution against a mirror graph at 5.6 ms median latency. Structurally broken queries are routed to a corrector that iterates structured error feedback through a language model. On seven CypherBench schemas (2348 questions, ACL 2025) the pipeline maintains generation accuracy on every model tested, confirming it operates as a safe defensive layer. The corrector achieves 81% to 95% success across five models (mean 89%). On a template-generated corpus across nine schemas the gate catches 100% of parse errors, 100% of constraint violations, and 100% of schema-reference errors in path queries with labelled endpoints, at zero false positives across 1135 queries. Property sibling-swaps where the substituted name is valid on the target label score 0%, marking the formal boundary where structural validation ends and semantic validation must begin. A planner-based cost gate flags catastrophic plan structures before execution.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.04645v1)
