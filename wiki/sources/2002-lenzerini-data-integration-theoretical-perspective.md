---
type: source
source_type: paper
kind: foundational
depth: reference
title: "Data Integration: A Theoretical Perspective"
authors: Maurizio Lenzerini
venue: PODS 2002, pp. 233–246
year: 2002
url: https://doi.org/10.1145/543613.543644
ingested: 2026-06-23
tags: [foundational, data-integration, mediated-architecture]
---

# Data Integration: A Theoretical Perspective

**ACM PODS 2002** · Maurizio Lenzerini · [doi:10.1145/543613.543644](https://doi.org/10.1145/543613.543644)

**Significance.** The canonical theory of data integration — defines the mediated schema and the **LAV vs GAV** mapping paradigms that underpin [[mediated-semantic-architecture]].

## Contribution (foundational)
Formalizes a data integration system as a triple ⟨G, S, M⟩: a **global (mediated) schema** G, a **source schema** S, and a **mapping** M between them. Two mapping approaches:
- **GAV (global-as-view)** — each global element is defined as a view over the sources; query processing is simple (unfolding), but adding/changing a source can force the global schema to be revised.
- **LAV (local-as-view)** — each source is described as a view over the global schema; query answering is harder (requires view-based query rewriting), but new sources are added by adding descriptions, *without* changing the mediated schema.
It establishes the semantics of query answering over incomplete/heterogeneous data (certain answers). The LAV property — extensibility under source change — is precisely why a semantic layer with source-described islands can "resolve to whatever islands are available."

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]]
- **Entities:** [[ontology-based-data-access]] · [[mediator-wrapper]]
