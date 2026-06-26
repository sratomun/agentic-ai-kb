---
type: entity
entity_type: protocol
tags: [agents, query-language, knowledge-graph]
created: 2026-06-23
updated: 2026-06-23
---

# Cypher

*The graph query language for property graphs (Neo4j) — ASCII-art pattern matching over nodes, relationships, and paths; the target formalism of text-to-Cypher.*

## What it is
Cypher expresses graph patterns declaratively, e.g. `MATCH (p:Person {name:"Tom Hanks"})-[:ACTED_IN]->(m:Movie) RETURN m.title`. It is the property-graph counterpart to SQL and is moving toward the ISO-GQL standard.

## Why it matters
Cypher is the executable target that makes a [[knowledge-graph]] queryable in natural language — the formalism under [[text-to-cypher]] and the engine of property-graph GraphRAG.

## Relationships
- target formalism of [[text-to-cypher]]
- queries [[knowledge-graph]] (property graphs)
- relational counterpart: SQL (see [[text-to-sql]])
- standardized by [[neo4j]]; benchmarked by [[text2cypher-dataset]] · [[cypherbench]]

## Cited by
- [[2024-12-13-arxiv-2412-10064-text2cypher-bridging-natural-language-graph-databases]]
- [[2026-06-12-arxiv-2606-14325-precise-text-to-cypher-grounded-kg-data-generation]]
