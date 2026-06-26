---
type: entity
entity_type: benchmark
tags: [agents, benchmark, nlu, data]
created: 2026-06-23
updated: 2026-06-23
---

# AMBROSIA

*Benchmark for parsing ambiguous questions into database queries — scope, attachment, and vagueness ambiguity that persists even with the database in context.*

## What it is
AMBROSIA (Saparina & Lapata, Edinburgh; NeurIPS 2024 D&B) tests whether text-to-SQL parsers recognize and interpret ambiguous requests. Databases are generated from scratch so ambiguity survives schema grounding; frontier LLMs struggle.

## Why it matters
The yardstick for the hard part of [[intent-grounding]]: even with structure available, models miss ambiguous intent. Motivates disambiguate-first pipelines.

## Relationships
- benchmark for [[intent-grounding]] and [[data-query-agents]]
- introduced alongside [[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later|Disambiguate First, Parse Later]]

## Cited by
- [[2024-06-27-arxiv-2406-19073-ambrosia-parsing-ambiguous-questions]]
- [[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later]]
