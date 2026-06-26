---
type: source
source_type: paper
kind: foundational
depth: reference
title: "Mediators in the Architecture of Future Information Systems"
authors: Gio Wiederhold
venue: IEEE Computer 25(3):38–49
year: 1992
url: https://doi.org/10.1109/2.121508
ingested: 2026-06-23
tags: [foundational, mediated-architecture, data-integration]
---

# Mediators in the Architecture of Future Information Systems

**IEEE Computer 25(3), 1992** · Gio Wiederhold · [doi:10.1109/2.121508](https://doi.org/10.1109/2.121508)

**Significance.** The origin of the **mediator** concept — the seminal source for the entire mediated-architecture lineage and for [[mediator-wrapper]].

## Contribution (foundational)
Wiederhold proposes that future information systems be built not as monoliths but from many small, interacting modules. A **mediator** is a software module occupying an explicit *middle layer* between data resources and applications: it encodes domain knowledge, and actively transforms, abstracts, and integrates lower-level data into information usable by a higher application layer. The companion idea — later formalized as the **wrapper** — encapsulates each heterogeneous source behind a uniform interface. This decomposition (wrappers expose sources; a mediator decomposes queries, allocates them, and integrates results) is the architectural blueprint that data integration, OBDA, and today's LLM-agent federation all re-instantiate.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]]
- **Entities:** [[mediator-wrapper]]
