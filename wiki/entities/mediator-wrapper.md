---
type: entity
entity_type: method
tags: [agents, method, data-integration]
created: 2026-06-23
updated: 2026-06-23
---

# Mediator–wrapper architecture

*The foundational pattern for querying heterogeneous sources: a mediator decomposes a query against a global view; per-source wrappers translate to each source's native interface.*

## What it is
Introduced by Wiederhold (1992): integration via small interacting components — **wrappers** that encapsulate each source behind a standard interface, and a **mediator** above them that decomposes queries, allocates them to wrappers, and integrates results. Recently revised for modern heterogeneous integration (the "mask" extension, arXiv 2208.12319).

## Why it matters
It is the structural backbone of [[mediated-semantic-architecture]]: the semantic layer is the mediator, the [[text-to-query-wrapper|text-to-query engines]] are the wrappers. Names exactly the "navigation map resolves, then fetch from islands" design.

## Foundational reference
- [[1992-wiederhold-mediators-architecture-future-information-systems|Wiederhold 1992]] — the origin of the mediator concept.
- Mediated-schema theory (LAV/GAV): [[2002-lenzerini-data-integration-theoretical-perspective|Lenzerini, PODS 2002]].
- Modern revision: [[2022-08-25-arxiv-2208-12319-mask-mediator-wrapper-heterogeneous-integration|Mask-Mediator-Wrapper]] (arXiv 2208.12319).

## Relationships
- backbone of [[mediated-semantic-architecture]]
- wrappers realized as [[text-to-query-wrapper]]
- complements [[ontology-based-data-access]] (ontology as the mediated schema)

## Cited by
- [[1992-wiederhold-mediators-architecture-future-information-systems]]
- [[2002-lenzerini-data-integration-theoretical-perspective]]
- [[2022-08-25-arxiv-2208-12319-mask-mediator-wrapper-heterogeneous-integration]]
