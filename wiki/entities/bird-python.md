---
type: entity
entity_type: benchmark
aliases: [BIRD-Python]
tags: [agents, benchmark, text-to-sql, text-to-python, evaluation]
created: 2026-06-22
updated: 2026-06-22
---

# BIRD-Python

*A cross-paradigm text-to-query benchmark that compares Text-to-Python and Text-to-SQL on equal footing.*

## What it is
BIRD-Python is a benchmark (Hu et al., 2026) derived from BIRD's 1,534-pair dev set, reconstructing SQL logic as Python/Pandas over CSVs and using an LLM-based Execution Accuracy validator. It isolates grounding failures from code-generation failures.

## Why it matters
Most enterprise data-query agents default to SQL, but Python/Pandas is equally viable. BIRD-Python's finding — that performance gaps come from missing domain context, not code-gen ability — tells teams where to invest: better grounding, not better models.

## Relationships
- variant of [[bird-benchmark]]
- evaluates [[data-query-agents]]
- part of [[agent-evaluation]]

## Cited by
- [[2026-01-22-arxiv-2601-15728v2-bird-python-text-to-python-vs-sql]]
