---
type: concept
tags: [agents, text-to-sql, data, semantic-layer]
created: 2026-06-21
updated: 2026-06-22
census_count: 50
kind: domain
---

# Data-query & text-to-SQL agents

*Agents that turn natural language into governed queries over structured data — text-to-SQL/NL2SQL, database and semantic-layer interfaces, analytics.*

## What it is
The bridge between natural language and an organization's data systems: agents that interpret intent, ground it to a schema, generate and refine a query, and return verified results. Closely tied to [[knowledge-graph]] (the semantic-layer contract) and extended by [[data-analysis-agents]].

## Why it matters
This is the practical home of the **"semantic layer"** question you raised — agents that translate intent into *governed* queries over real schemas, not a chat box over a warehouse. The enterprise pull is obvious, benchmarks are maturing ([[bird-benchmark|BIRD]], [[spider-benchmark|Spider 2.0]]), and the 2026 work is reframing what "good" even means here.

## What the evidence shows
**2025 foundations.** The winning text-to-SQL pattern became **multi-agent + alignment**: OpenSearch-SQL decomposes the task into Preprocessing → Extraction → Generation → Refinement with a consistency-alignment module that reduces instruction-following failures and hallucination (→ [[2025-02-19-arxiv-2502-14913v1-opensearch-sql-enhancing-text-to-sql-with-dynamic]]).

**2026 developments — the metric is the story.** Recent work argues accuracy alone is the wrong target:
- **Grounding, not code-gen, is the bottleneck** — Text-to-Python reaches parity with SQL once intent is clarified; annotation noise must be cleaned first → [[2026-01-22-arxiv-2601-15728v2-bird-python-text-to-python-vs-sql]] (cf. [[bird-python]]).
- **At scale, cost + latency matter as much as correctness** — VES*/VCES/CVQ price efficiency, and accuracy spreads models far more than execution metrics → [[2026-02-25-arxiv-2602-21480v4-text-to-big-sql-cost-metrics]].

## Relationships
- uses [[tool-use]], [[knowledge-graph]], [[agentic-rag]]
- the execution surface for [[intent-grounding]]; queries the [[metrics-layer]]
- the agentic application of [[semantic-parsing]] ([[text-to-sql]] + [[text-to-cypher]])
- operates within [[mediated-semantic-architecture]] (mediator + wrappers)
- benchmarks: [[bird-benchmark]], [[bird-python]], [[spider-benchmark]]
- extended by [[data-analysis-agents]]
- evaluation nuances in [[agent-evaluation]]
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **76** · [[2025-02-19-arxiv-2502-14913v1-opensearch-sql-enhancing-text-to-sql-with-dynamic|OpenSearch-SQL: Enhancing Text-to-SQL with Dynamic Few-shot and Consistency Ali...]]
