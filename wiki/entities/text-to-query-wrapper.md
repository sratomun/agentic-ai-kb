---
type: entity
entity_type: method
tags: [agents, method, semantic-parsing]
created: 2026-06-23
updated: 2026-06-23
---

# Text-to-query wrapper

*The per-island adapter that turns a logical sub-query into a storage-native query — text-to-SQL, text-to-Cypher, vector search, or text-to-API — selected by the island's storage paradigm.*

## What it is
The "wrapper" half of [[mediator-wrapper]], implemented as a [[semantic-parsing]] engine matched to each storage type: relational/analytical → [[text-to-sql]]; graph → [[text-to-cypher]]; vector → embed + similarity + rerank; app/SOR → text-to-API tool call. Each is grounded against its island's own semantic description + schema.

## Why it matters
This is what makes "could not care less about storage" true at modeling time: the business layer stays storage-agnostic and the wrapper descends to physical. But the *planner* must pick the wrapper by capability — a vector store answers "find similar," a graph answers traversal, SQL answers aggregation — so storage-transparency holds for the modeler, capability-awareness for the planner.

## Relationships
- the wrapper in [[mediator-wrapper]] / [[mediated-semantic-architecture]]
- instances: [[text-to-sql]] · [[text-to-cypher]] · (vector retrieval) · text-to-API
- family hub: [[semantic-parsing]]
- selected by source-selection in [[intent-routing]]

## Cited by
- [[2026-05-28-arxiv-2605-29250-omniretrieval-unified-retrieval-heterogeneous]]
- [[2025-10-18-arxiv-2510-16470-declarative-nl-queries-over-heterogeneous-data]]
