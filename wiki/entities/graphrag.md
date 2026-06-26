---
type: entity
entity_type: method
tags: [agents, method]
created: 2026-06-21
updated: 2026-06-22
census_count: 33
---

# GraphRAG

*Graph-structured RAG — retrieving over entity-relation graphs instead of flat text chunks for multi-hop and global queries.*

## What it is
GraphRAG retrieves information from a knowledge graph (entities, relations, community summaries) rather than flat vector chunks, enabling multi-hop and global sensemaking queries that dense retrieval misses. Mentioned in ~33 of 2026 H1 census papers.

## Why it matters
For enterprise use cases with rich relational data — org charts, product catalogs, compliance networks — GraphRAG consistently outperforms flat RAG. It's the architecture to consider when a standard RAG pipeline gives incoherent multi-hop answers.

## Relationships
- method bridging [[knowledge-graph]] and [[agentic-rag]]
- contrast with flat retrieval in [[tool-use]]
