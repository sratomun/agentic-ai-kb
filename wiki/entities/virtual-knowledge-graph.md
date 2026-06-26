---
type: entity
entity_type: method
tags: [agents, method, obda, knowledge-graph]
created: 2026-06-23
updated: 2026-06-23
aliases: [VKG, virtual knowledge graph]
---

# Virtual Knowledge Graph (VKG)

*The graph reframing of OBDA: data stays in place in its sources and is exposed as a virtual graph through declarative mappings, queried (e.g. SPARQL→SQL) without materialisation.*

## What it is
A VKG presents heterogeneous sources as one graph *without copying the data* — each node/edge is a declaratively-mapped view over a source table or API. Queries against the virtual graph are rewritten to the sources at runtime (Xiao et al. 2019; tooling such as Ontop).

## Why it matters
VKG is how the [[mediated-semantic-architecture]] avoids a sync problem: instead of ETL-ing islands into one store, you expose them as a virtual graph over their semantic descriptions. The enterprise reasoner [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner|HEAR]] builds its data layer exactly this way (nodes = semantic views of DB tables / API endpoints, data in-place).

## Foundational reference
- [[2019-xiao-virtual-knowledge-graphs-overview|Xiao et al. 2019]] — the canonical VKG overview.

## Relationships
- graph form of [[ontology-based-data-access]]
- realises [[mediated-semantic-architecture]] without materialisation
- a [[knowledge-graph]] projected over live sources
- queried via [[text-to-cypher]] / SPARQL ([[semantic-parsing]])

## Cited by
- [[2019-xiao-virtual-knowledge-graphs-overview]]
- [[2008-poggi-linking-data-to-ontologies]]
- [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner]]
