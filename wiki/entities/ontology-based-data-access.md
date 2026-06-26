---
type: entity
entity_type: method
tags: [agents, method, obda, data-integration]
created: 2026-06-23
updated: 2026-06-23
aliases: [OBDA, OBDM, ontology-based data management]
---

# Ontology-Based Data Access (OBDA)

*Accessing heterogeneous data through a shared ontology linked to sources by declarative mappings; queries are posed in ontology terms and rewritten to the sources.*

## What it is
An OBDA specification is a triple ⟨ontology (TBox), source schema, mapping⟩ (Poggi et al. 2008). Users query the ontology — a rich business-domain model — and the system rewrites those queries to the underlying sources, deriving extra answers via reasoning. Lenzerini's broader framing is Ontology-Based Data Management (OBDM, 2011). It is the formal version of "a semantic layer aligned to source semantic descriptions."

## Why it matters
OBDA *is* the exec's logical-layer-over-islands model, with decades of theory behind it: the ontology is the navigation map, the mappings are the semantic alignments, query rewriting is the agent's resolution-to-fetch. The basis of [[mediated-semantic-architecture]].

## Foundational reference
- [[2008-poggi-linking-data-to-ontologies|Poggi et al. 2008]] — established the OBDA framework.
- [[2018-xiao-ontology-based-data-access-survey|Xiao et al., OBDA Survey 2018]] — the standard survey.
- Mediated-schema theory (LAV/GAV): [[2002-lenzerini-data-integration-theoretical-perspective|Lenzerini, PODS 2002]].

## Relationships
- formal basis of [[mediated-semantic-architecture]]
- graph reframing: [[virtual-knowledge-graph]]
- query rewriting → [[semantic-parsing]] wrappers
- ontology lives in [[knowledge-graph]]

## Cited by
- [[2008-poggi-linking-data-to-ontologies]]
- [[2018-xiao-ontology-based-data-access-survey]]
- [[2002-lenzerini-data-integration-theoretical-perspective]]
- [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner]]
