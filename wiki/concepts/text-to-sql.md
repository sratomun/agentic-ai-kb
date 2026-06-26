---
type: concept
tags: [agents, text-to-sql, semantic-parsing, data]
created: 2026-06-23
updated: 2026-06-23
kind: domain
---

# Text-to-SQL

*Translating natural language into executable SQL over relational schemas — the most-studied child of [[semantic-parsing]], and the relational sibling of [[text-to-cypher]].*

## What it is
Mapping a question plus a relational schema to a runnable SQL query. The classic benchmarks are [[spider-benchmark|Spider]] (cross-domain) and [[bird-benchmark|BIRD]] (large, messy, value-grounded). This node is the *task*; the *agentic application* — multi-step querying, semantic-layer/API grounding, recovery loops — lives in [[data-query-agents]].

## Why it matters
Text-to-SQL is the workhorse of natural-language analytics, and the lesson the production work keeps returning is governance: don't let the model own the business logic. In the exec's world this is the research backing for querying a metrics/semantic-layer vault rather than free-handing SQL.

## What the evidence shows
**Foundations.** Real-world text-to-SQL is under-specified until phrases are grounded in how the database stores values; grounding "too early" is the dominant failure. Keeping grounding hypotheses open and letting **execution** decide — then caching the verified grounding as reusable memory — beats one-shot grounding (**55.2% on RealEHR**, 97.8% memory reuse → [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|GATE]]). Ambiguity is the other foundation: it survives schema context ([[2024-06-27-arxiv-2406-19073-ambrosia-parsing-ambiguous-questions|AMBROSIA]]) and is best handled by disambiguating in natural language first ([[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later|Disambiguate First, Parse Later]]).

**Recent developments — from SQL to governed interfaces.** Production has moved past raw SQL toward **governed APIs / semantic layers**: plan over defined metrics and permissions instead of generating SQL, keeping definitions and audit outside the model (**77.22% E2E** → [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL]]). And the formalism boundary is dissolving — joint SQL+Cypher training transfers both ways ([[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM]]). Industry benchmarks report a governed semantic layer taking LLM accuracy from ~40% to ~83% (vendor-reported; weight accordingly).

## Relationships
- child of [[semantic-parsing]]; sibling of [[text-to-cypher]]
- agentic application: [[data-query-agents]]
- grounded against [[metrics-layer]]; resolved via [[intent-grounding]]
- benchmarks: [[spider-benchmark]] · [[bird-benchmark]]

## Key papers (curated by relevance)
<!-- Curated from the papers this node cites + backlinks; per-paper citation counts not in the 2025–26 census window. Ordered by velocity/recency. -->
- [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|Bootstrapping Semantic Layer from Execution for Text-to-SQL]]
- [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL: An Agentic LLM System for Governed Enterprise Anal…]]
- [[2025-12-21-arxiv-2512-18622v1-a-multi-agent-text2sql-framework-using-small-language-models-and-execu|A Multi-agent Text2SQL Framework using Small Language Models and Execu…]]
- [[2025-12-16-arxiv-2512-14043v1-evaluating-small-language-models-for-agentic-on-farm-decision-support|Evaluating Small Language Models for Agentic On-Farm Decision Support …]]
- [[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM: Unifying Tabular and Graph Reasoning with Reinforcement Le…]]
- [[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later|Disambiguate First, Parse Later: Generating Interpretations for Ambigu…]]
- [[2024-06-27-arxiv-2406-19073-ambrosia-parsing-ambiguous-questions|AMBROSIA: A Benchmark for Parsing Ambiguous Questions into Database Qu…]]
