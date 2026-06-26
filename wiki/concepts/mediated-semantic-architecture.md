---
type: concept
tags: [agents, mediated-architecture, semantic-layer, data-integration, obda]
created: 2026-06-23
updated: 2026-06-23
kind: hub
aliases: [mediated semantic layer, mediated semantic architecture]
---

# Mediated semantic layer

*A stable business semantic layer over volatile heterogeneous data islands, bound by semantic alignments, with per-island text-to-query wrappers — so an agent resolves an utterance in domain terms and fetches from whatever sources can serve it.*

## What it is
The architecture under [[intent-grounding]]: separate **what the business means** (a semantic layer of concepts, entities, relationships, synonyms, conflicts) from **where/how the data lives** (each data island with its own semantic description), connected by **semantic alignments** (mappings). An agent resolves an utterance against the semantic layer, then mediates down through the alignments to fetch from the relevant islands. This is the classic **mediator–wrapper** pattern ([[1992-wiederhold-mediators-architecture-future-information-systems|Wiederhold 1992]]) and **ontology-based data access** (OBDA; [[2008-poggi-linking-data-to-ontologies|Poggi et al. 2008]], [[2018-xiao-ontology-based-data-access-survey|Xiao et al., OBDA Survey 2018]]) reborn for LLM agents — the semantic layer is the *mediator*, the per-island [[text-to-query-wrapper|text-to-query engines]] are the *wrappers*.

## Why it matters
This is the decomposition that makes an enterprise intent engine maintainable. Three payoffs: (1) **storage independence** — the business layer is agnostic to SQL DB / analytical DB / vector DB / graph DB; each island is reached by the appropriate [[semantic-parsing|text-to-query]] engine. (2) **Source substitutability** — describing each island *in terms of the semantic layer* (the LAV side of data integration; [[2002-lenzerini-data-integration-theoretical-perspective|Lenzerini, PODS 2002]]) means adding or dropping an island is a description change, not a rewrite of the business map. That robustness is exactly what "resolve to whatever relevant islands are available" requires. (3) **Drift isolation** — physical change is absorbed at the alignment tier; the business map only changes when the *business* changes. The same separation that the [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|governed-API]] work argues (LLM as planner, not business-logic store) generalized to many sources.

## What the evidence shows
**The mediator argument, in pure form.** The leading principle is *don't homogenize sources — meet each on its own terms*: [[2026-05-28-arxiv-2605-29250-omniretrieval-unified-retrieval-heterogeneous|OmniRetrieval]] takes any NL query, identifies the right sources, and **dispatches source-native queries to native engines** across 13 datasets / 309 knowledge bases, beating single-source baselines while preserving each source's structural affordances (schemas, ontologies, operators). This *is* the mediator–wrapper claim, validated.

**Declarative beats agentic for the fetch.** Treating heterogeneous DB+API access declaratively — APIs as SQL virtual tables/UDFs — beats both imperative Python and a ReAct agent: **0.689 vs 0.357 accuracy at ~half the latency** ([[2025-10-18-arxiv-2510-16470-declarative-nl-queries-over-heterogeneous-data|siwarex / IBM]]). The lesson: separate declarative intent (the logical query) from execution planning (the wrappers), and let mature query optimization do the rest.

**Source selection is its own routing problem.** Decoupling **schema routing** from query generation scales NL querying to massive multi-database settings ([[2023-12-06-arxiv-2312-03463-dbcopilot-schema-routing-massive-databases|DBCopilot]]) — this is the data-source-selection step inside grounding, distinct from model/tool routing in [[intent-routing]]. Capability-driven dispatch generalizes it: advertise each source/agent's capabilities as vectors and route by them ([[2025-09-24-arxiv-2509-20175-federation-of-agents-capability-fabric|Federation of Agents]]).

**Enterprise instantiation over real systems.** [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner|HEAR]] virtualizes BPM/ERP/SRM/WMS as a **Virtual Knowledge Graph** ([[2019-xiao-virtual-knowledge-graphs-overview|Xiao et al. 2019]]) — each node a semantic view of a DB table or API endpoint, data staying in-place via declarative mappings — and reasons over n-ary business rules to hit **94.7%** on root-cause questions. The single-retrieval-plane variant fuses vector + KG + full-text + relational backends, each with its own trade-offs ([[2025-09-12-arxiv-2509-21336-hetarag-heterogeneous-data-stores|HetaRAG]]); agentic analytics compiles an NL query into a semantic plan of relational + semantic operators over structured and unstructured data ([[2025-08-07-arxiv-2508-05002-agenticdata-heterogeneous-data|AgenticData]]). Benchmarks and surveys now frame the whole space ([[2025-09-02-arxiv-2509-02473-fdabench-data-agents-heterogeneous|FDABench]]; [[2025-09-28-arxiv-2509-23988-llm-agent-as-data-analyst-survey|LLM/Agent-as-Data-Analyst]]; [[2025-05-24-arxiv-2505-18458-survey-llm-x-data|LLM × DATA]]).

**Foundational caveat.** The spine is decades-old database theory (mediator–wrapper, LAV/GAV, OBDA, VKG); the LLM era supplies the wrappers (text-to-query) and the planner (an agent), not the architecture. Cite the classics — this is a re-instantiation, not an invention.

## Includes (sub-themes folded here)
Folds in: the logical/business layer, semantic alignments (LAV/GAV mappings), source descriptions & capability declaration, source selection / data-source routing, and the multi-engine federation executor. Per-formalism translation lives in [[semantic-parsing]]; the structured target lives in [[knowledge-graph]] / [[metrics-layer]].

## Relationships
- the architecture realizing [[intent-grounding]]
- mediator pattern: [[mediator-wrapper]]; data access: [[ontology-based-data-access]]; graph reframing: [[virtual-knowledge-graph]]
- wrappers are [[text-to-query-wrapper]] (the [[semantic-parsing]] family)
- source selection is a form of [[intent-routing]] (over data sources, not models)
- targets [[knowledge-graph]] + [[metrics-layer]] over [[data-query-agents]]
- maintained by the alignment-tier drift loop (see [[knowledge-graph]] build/maintain)

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. Citations from census/source-note frontmatter. -->
- **22** · 2.5/mo · [[2025-09-28-arxiv-2509-23988-llm-agent-as-data-analyst-survey|LLM/Agent-as-Data-Analyst: A Survey]]
- **21** · 2.0/mo · [[2025-08-07-arxiv-2508-05002-agenticdata-heterogeneous-data|AgenticData: An Agentic Data Analytics System for Heterogeneous Da…]]
- **6** · 0.6/mo · [[2025-09-02-arxiv-2509-02473-fdabench-data-agents-heterogeneous|FDABench: A Benchmark for Data Agents on Analytical Queries over H…]]
- **5** · 0.6/mo · [[2025-09-24-arxiv-2509-20175-federation-of-agents-capability-fabric|Federation of Agents: A Semantics-Aware Communication Fabric for L…]]
- **1** · 0.1/mo · [[2025-05-24-arxiv-2505-18458-survey-llm-x-data|A Survey of LLM x DATA]]
- **0** · [[2025-10-18-arxiv-2510-16470-declarative-nl-queries-over-heterogeneous-data|Declarative Techniques for NL Queries over Heterogeneous Data]]
- **0** · [[2026-05-14-arxiv-2605-14259-hypergraph-enterprise-agentic-reasoner|Hypergraph Enterprise Agentic Reasoner over Heterogeneous Business…]]
