---
type: source
source_type: paper
kind: foundational
depth: reference
title: "Linking Data to Ontologies"
authors: Poggi, Lembo, Calvanese, De Giacomo, Lenzerini, Rosati
venue: Journal on Data Semantics X (LNCS 4900), pp. 133–173
year: 2008
url: https://doi.org/10.1007/978-3-540-77688-8_5
ingested: 2026-06-23
tags: [foundational, obda, data-integration]
---

# Linking Data to Ontologies

**Journal on Data Semantics X, 2008** · Poggi, Lembo, Calvanese, De Giacomo, Lenzerini, Rosati · [doi:10.1007/978-3-540-77688-8_5](https://doi.org/10.1007/978-3-540-77688-8_5)

**Significance.** The paper that established the **Ontology-Based Data Access** framework — the formal basis of [[ontology-based-data-access]].

## Contribution (foundational)
Defines an OBDA system as an ontology (a TBox, expressed in a tractable description logic — the DL-Lite family) linked to autonomous relational data sources by declarative **mappings**. Two key ideas: (1) **query answering by rewriting** — a query over the ontology is rewritten (perfect rewriting) into a query the sources can answer (ultimately SQL), so the data need not be moved into the ontology; and (2) the **impedance mismatch** between data values in sources and objects in the ontology is bridged by the mappings. DL-Lite is chosen precisely so that rewriting stays first-order/SQL-expressible (tractable in data complexity). This is the ⟨ontology, sources, mappings⟩ triple that the exec's logical-layer-aligned-to-island-descriptions model instantiates.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]]
- **Entities:** [[ontology-based-data-access]] · [[virtual-knowledge-graph]]
