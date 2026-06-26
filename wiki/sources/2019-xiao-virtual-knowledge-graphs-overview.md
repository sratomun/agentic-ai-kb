---
type: source
source_type: paper
kind: foundational
depth: full-text
title: "Virtual Knowledge Graphs: An Overview of Systems and Use Cases"
authors: Guohui Xiao, Linfang Ding, Benjamin Cogrel, Diego Calvanese (KRDB, Free University of Bozen-Bolzano)
venue: Data Intelligence 1(3):201–223
year: 2019
url: https://doi.org/10.1162/dint_a_00011
html: https://direct.mit.edu/dint/article/1/3/201/9978/Virtual-Knowledge-Graphs-An-Overview-of-Systems-and
ingested: 2026-06-23
read_via: Claude-in-Chrome (MIT Press open-access HTML; full body read section by section)
tags: [foundational, obda, knowledge-graph, mediated-architecture]
---

# Virtual Knowledge Graphs: An Overview of Systems and Use Cases

**Data Intelligence 1(3), 2019** · Xiao, Ding, Cogrel, Calvanese · [doi:10.1162/dint_a_00011](https://doi.org/10.1162/dint_a_00011)

**Significance.** The canonical VKG overview — the graph-native packaging of OBDA that [[virtual-knowledge-graph]] is built on, and the reference [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner|HEAR]] cites for its data layer. Full text read via Chrome 2026-06-23; it confirms (no corrections needed) the prior canonical summary and adds the specifics below.

## Abstract (verbatim)
"In this paper, we present the virtual knowledge graph (VKG) paradigm for data integration and access, also known in the literature as Ontology-based Data Access. Instead of structuring the integration layer as a collection of relational tables, the VKG paradigm replaces the rigid structure of tables with the flexibility of graphs that are kept virtual and embed domain knowledge. We explain the main notions of this paradigm, its tooling ecosystem and significant use cases in a wide range of applications. Finally, we discuss future research directions."

## From the paper (full-text)
**The paradigm = V + G + K.** *Virtualization* — users see a conceptual global schema defined by views over sources; the views are "not materialized, but are kept virtual," so you query without paying storage/time to build the graph. *Graph* — objects/values are nodes, properties are edges; two graphs integrate by union + merging identical nodes (`owl:sameAs` / canonical IDs), avoiding ad-hoc relational-merge complexity. *Knowledge* — the graph is enriched with domain axioms (hierarchies, domains/ranges, mandatory properties) enabling inference. **Crucially the KG is never built**: mapping queries "are not executed to actually construct the RDF knowledge graph… Instead, they are used to suitably rewrite user queries posed over the ontology in terms of queries over the sources."

**Formal framework.** A VKG specification is **P = (O, M, S)** — ontology, mapping, source schema; with a compliant DB *D* it forms a VKG instance. Ontology language **OWL2**, with the OBDA sublanguage **OWL2QL** (formal counterpart the **DL-Lite** family — lightweight so query answering with domain knowledge stays efficient at scale). A mapping is a set of assertions each pairing a **SQL query over S** with an **RDF triple template**; standard mapping language **W3C R2RML** (+ Direct Mapping). **Query answering = reformulation:** a SPARQL query is *rewritten w.r.t. the ontology* then *unfolded w.r.t. the mapping* into SQL executed on D. The naive workflow is "highly inefficient"; viability needs optimizations — compile the ontology into the mapping offline, exploit data constraints to simplify the unfolded SQL, and cost-based execution planning.

**Systems surveyed.** **Ontop** (the authors' system; Free Univ. Bozen-Bolzano / Ontopic; Apache-2; R2RML + compact mapping language; OWL2QL reasoning; many JOIN/UNION/OPTIONAL optimizations; spatial/temporal/MongoDB prototypes) — the most-deployed in the use cases. Also **Mastro** (Sapienza/OBDA Systems), **Morph** (UPM), **D2RQ** (historical pioneer), **Stardog**, **Oracle Spatial & Graph**, **Ultrawrap** (Capsenta). Mapping engineering: bootstrappers (BootOX, MIRROR, COMA, Karma; RODI benchmark) and editors (Protégé plugins, Map-On, RMLEditor). Federation: SQL (Exareme, Denodo, Dremio, Teiid) and SPARQL (SemaGrow).

**Use cases.** Oil & gas — **Equinor/Statoil** (the Optique platform: BootOX + Ontop + Exareme + OptiqueVQS, freeing geologists from IT-mediated queries); **Siemens** turbine/generator diagnostics over static + sensor data; **Italian Public Debt** Directorate (Mastro Studio); **Constitute** (196+ constitution databases, Ultrawrap; launched at the UN 2013); healthcare (Diabetes Mellitus Ontology + Ontop auto-identifies diabetic patients across ~1,000 active patients; HL7 via Morph); **maritime security / RMSAS** (Ontop-spatial, GeoSPARQL→SQL, integrating vessel metadata + open data + radar/satellite at **~1,000 vessel positions per second**); process mining (OnProm → XES logs); temporal access to **MIMIC-III** critical-care data (Ontop-temporal) for trial-patient selection.

**Terminology.** The paper leads with **VKG** and treats **OBDA** as the established formal-setting synonym ("also known in the literature as ontology-based data access").

**Takeaway.** The authoritative statement of "logical graph over live sources, queried by rewriting, no ETL" — and a roster of real industrial deployments. The direct evidence that the mediated-semantic-architecture's keep-data-in-place tier is a mature, shipped pattern, not a proposal.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[knowledge-graph]]
- **Entities:** [[virtual-knowledge-graph]] · [[ontology-based-data-access]]

## Provenance
Read via Claude-in-Chrome from the MIT Press open-access HTML (full body, section by section). The sciengine.com PDF link provided by the user is a direct file download and would not render in-browser; the MIT Press HTML is the same article (DOI 10.1162/dint_a_00011).
