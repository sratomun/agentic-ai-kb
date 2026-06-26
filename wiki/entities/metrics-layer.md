---
type: entity
entity_type: method
tags: [agents, method, semantic-layer, data]
created: 2026-06-23
updated: 2026-06-23
aliases: [analytics semantic layer, metrics semantic layer]
---

# Metrics layer

*The governed analytics island — metrics, dimensions, and their formulas defined once over a warehouse/marts — that serves the "measure" facet. (In industry this is often called "the semantic layer"; in this wiki the top-tier business model is the [[mediated-semantic-architecture|semantic layer]], and this is one island beneath it.)*

## What it is
A governed definition layer over relational/analytical stores: metrics (as formulas), dimensions, and the entities they hang on, defined once and reused. The LLM decomposes a question into the layer's defined metrics + dimensions rather than writing raw SQL.

## Why it matters
It is the island that answers *measure* questions, reached through the [[text-to-sql]] wrapper. Grounding NL in defined metrics (not free-form SQL) is what lifts analytics accuracy and keeps numbers consistent — industry benchmarks report ~40% → ~83% with a governed metrics layer. Mirrors the exec's `sem:` metrics vault: the metric definitions are the measure-facet taxonomy.

## Relationships
- an island under [[mediated-semantic-architecture]] (distinct from the top-tier semantic layer / business model)
- serves the *measure* access pattern of [[intent-grounding]]
- reached via the [[text-to-sql]] wrapper ([[text-to-query-wrapper]])
- queried by [[data-query-agents]]; complements [[knowledge-graph]] (the *relate* island)

## Cited by
- [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics]]
- [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql]]
- [[2024-11-25-arxiv-2412-07786-towards-agentic-schema-refinement]]
