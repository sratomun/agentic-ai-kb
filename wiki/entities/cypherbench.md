---
type: entity
entity_type: benchmark
tags: [agents, benchmark, knowledge-graph]
created: 2026-06-23
updated: 2026-06-23
---

# CypherBench

*Benchmark for precise LLM retrieval over full-scale knowledge graphs via Cypher — property-graph views over Wikidata (11 graphs, 7.8M entities, 10k+ questions).*

## What it is
CypherBench (Megagon Labs, ACL 2025) proposes property-graph *views* on top of RDF graphs (Wikidata/Freebase), whose oversized schemas and identifiers make them hard for LLMs, so they can be queried efficiently with Cypher.

## Why it matters
The benchmark for *encyclopedic-scale* text-to-Cypher and the proof that property-graph views beat raw RDF for LLM retrieval — central to graph-grounded GraphRAG. From the same lab as [[2025-08-29-arxiv-2509-04472-recap-rewriting-conversations-intent-understanding|RECAP]].

## Relationships
- benchmark for [[text-to-cypher]] and [[knowledge-graph]] retrieval
- targets [[cypher]]; companion to [[text2cypher-dataset]]
- used by [[2026-06-12-arxiv-2606-14325-precise-text-to-cypher-grounded-kg-data-generation|CYQUARK]] · [[2025-11-11-arxiv-2511-08274-multi-agent-graphrag-text-to-cypher-lpg|Multi-Agent GraphRAG]]

## Cited by
- [[2024-12-24-arxiv-2412-18702-cypherbench-precise-retrieval-knowledge-graphs]]
