---
type: source
source_type: arxiv
title: "AgentNLQ: A General-Purpose Agent for Natural Language to SQL"
authors: Olena Bogdanov, Yeunji Jung, Chandra Dhir, Pareekshitreddy Gaddam et al.
url: https://arxiv.org/abs/2605.19010v1
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [data-query-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AgentNLQ: A General-Purpose Agent for Natural Language to SQL

**arXiv:** [2605.19010v1](https://arxiv.org/abs/2605.19010v1) · 2026-05-18 · cs.AI
**Authors:** Olena Bogdanov, Yeunji Jung, Chandra Dhir, Pareekshitreddy Gaddam et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Natural language to SQL (NL2SQL) conversion is an important problem for researchers and enterprises due to the ubiquitous importance of relational databases in broad-ranging practical problems. Despite the rapid advancements in the capabilities of LLMs, NL2SQL has not reached parity in accuracy with human expert SQL writers, hence needing additional improvements in NL2SQL algorithms. This study presents a new multi-agent method for NL2SQL that achieves 78.1% semantic accuracy on the BIg Bench for LaRge-scale Database (BIRD) benchmark. Our method leverages a semantically enriched representation of user-provided schema, adds user-provided business rules, and produces accurate SQL queries. The main contributions of this study are (a) We designed an optimized new orchestrator in a multi-agent solution that uses LLMs to plan, orchestrate, reflect, and self-correct to generate accurate SQL queries, (b) We developed an advanced schema enrichment method that creates context-aware metadata to improve accuracy, and (c) We demonstrated the accuracy and generalizability of the method across different domains and datasets by evaluating it on the BIRD-SQL benchmark.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.19010v1)
