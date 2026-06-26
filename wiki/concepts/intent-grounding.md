---
type: concept
tags: [agents, intent-grounding, knowledge-graph, semantic-layer, nlu]
created: 2026-06-23
updated: 2026-06-23
kind: crosscutting
---

# Intent grounding

*Resolving user intent against a structure — an ontology, knowledge graph, or analytics semantic layer — instead of a flat label, so a smaller model stays accurate and the answer stays governed.*

## What it is
The bridge between [[intent-understanding]] and structured data. Rather than classify an utterance into one label, intent grounding maps it onto a **defined structure**: entities/relations in a [[knowledge-graph]], or metrics/dimensions in an analytics **[[metrics-layer]]**. The model's job shrinks from "produce the answer" to "decompose intent into the right pieces of a governed schema." It borders entity linking, semantic parsing (text-to-SQL / text-to-Cypher), and [[data-query-agents]].

## Why it matters
This is the resolution of the whole intent arc. The throughline of [[intent-understanding]] was *stop forcing intent into one flat label* — a semantic layer / KG is **the structured target you resolve into instead**, and it buys governance, consistency, and small-model efficiency for free. For the exec this is the most directly load-bearing thread: it is exactly the pattern of a metrics/semantic-layer vault — **the metric definitions are the intent taxonomy**. The production lesson is blunt: the LLM should *not* hold the business logic; it should be a planner over a governed structure that owns the definitions, permissions, and audit ([[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL]]).

## What the evidence shows
**Foundations — symbolic structure makes the small model competitive.** Grounding intent in an ontology lets a 3B model approach GPT-4 on multi-intent reads ([[2025-11-24-arxiv-2511-19780v1-noem3a-neuro-symbolic-multi-intent-understanding|NOEM³A]], 85% vs 90%); neuro-symbolic intent inference with theorem provers beats pure-LLM agents ([[2026-01-13-arxiv-2601-08742v1-inferring-latent-intentions-att-nli|Att-NLI]]). The binding step is **entity linking** — mapping ambiguous mentions to canonical KB entities, now done zero-shot ([[2026-01-08-arxiv-2601-05192-lela-zero-shot-entity-linking|LELA]]) and KG-triple-enhanced ([[2025-04-21-arxiv-2504-15135-kgmel-kg-enhanced-multimodal-entity-linking|KGMEL]]). And the ontology itself can be auto-derived from unstructured docs ([[2025-05-31-arxiv-2506-00664-ontorag-automated-ontology-derivation|OntoRAG]], 85% comprehensiveness win vs vector RAG).

**The analytics semantic layer — NL intent → governed metrics, not raw SQL.** This is the production face. Define metrics, dimensions, and entities once; the LLM decomposes the question against them. Dialpad's **Analytic Agent** plans over governed analytics *APIs* (not SQL), grounding "Support team in Seattle" to a permissioned entity and delegating dates to deterministic code — **77.22% E2E, 96.67% execution**, with the explicit lesson that business logic lives outside the model ([[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL]]). Where the layer doesn't exist, **bootstrap it from execution**: keep grounding hypotheses open, run them, keep the one the data supports, cache it (**GATE**, 97.8% memory reuse, 99.5% update accuracy → [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|Bootstrapping Semantic Layer]]). The layer can be *discovered* by collaborating agents as interpretable views ([[2024-11-25-arxiv-2412-07786-towards-agentic-schema-refinement|Agentic Schema Refinement]]), span SQL *and* graph formalisms ([[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM]], Text2Cypher +73.1%), and even make *intent itself a first-class KG node* ([[2025-05-16-arxiv-2505-10900-ikgr-intent-knowledge-graph-recommender|IKGR]], Capital One).

**The hard part is still ambiguity.** Even with the database in context, frontier models fail to recognize ambiguous intent — scope, attachment, vagueness ([[2024-06-27-arxiv-2406-19073-ambrosia-parsing-ambiguous-questions|AMBROSIA]]). The fix mirrors the clarification thread: **disambiguate in natural language first, validate interpretations by execution, then parse** ([[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later|Disambiguate First, Parse Later]]). Standardized intent ontologies (RDFS/SPARQL) push the same decoupling into operations ([[2026-05-26-arxiv-2605-27743-standardized-ontology-intent-based-security|Intent-Based Security Ontology]]).

**Caveat.** The biggest accuracy lever here is industry-reported, not peer-reviewed: dbt's 2026 benchmark puts LLM accuracy at **~40% without a semantic layer vs 83% with one** (text-to-SQL 32.7%→64.5%). Directionally consistent with the papers, but it's a vendor number — weight accordingly.

## Relationships
- grounds the output of [[intent-understanding]] (resolve intent → structure)
- structured target: [[knowledge-graph]] · [[metrics-layer]]
- realized by [[data-query-agents]] (text-to-SQL / text-to-Cypher / governed APIs)
- executed by [[semantic-parsing]] (NL → runnable query)
- architecturally realized by [[mediated-semantic-architecture]] (semantic layer ↔ alignments ↔ islands)
- ambiguity handling shared with the clarification thread in [[intent-understanding]] and with [[agentic-rag]]
- method: entity linking ([[entity-linking]]); benchmark: [[ambrosia]]
- governance tie-in: [[governance-gap]], [[agent-security]]

## Key papers (curated by relevance)
<!-- Curated from the papers this node cites + backlinks; per-paper citation counts not in the 2025–26 census window. Ordered by velocity/recency. -->
- [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|Bootstrapping Semantic Layer from Execution for Text-to-SQL]]
- [[2026-05-26-arxiv-2605-27743-standardized-ontology-intent-based-security|A Standardized Ontology for Intent-Based Security Management in Autono…]]
- [[2026-05-20-arxiv-2605-21027-beyond-text-to-sql-governed-enterprise-analytics|Beyond Text-to-SQL: An Agentic LLM System for Governed Enterprise Anal…]]
- [[2026-01-13-arxiv-2601-08742v1-inferring-latent-intentions-att-nli|Inferring Latent Intentions: Attributional Natural Language Inference …]]
- [[2026-01-08-arxiv-2601-05192-lela-zero-shot-entity-linking|LELA: A Modular Coarse-to-Fine Approach to Zero-Shot Entity Linking]]
- [[2025-11-24-arxiv-2511-19780v1-noem3a-neuro-symbolic-multi-intent-understanding|NOEM$^{3}$A: A Neuro-Symbolic Ontology-Enhanced Method for Multi-Inten…]]
- [[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM: Unifying Tabular and Graph Reasoning with Reinforcement Le…]]
- [[2025-05-31-arxiv-2506-00664-ontorag-automated-ontology-derivation|OntoRAG: Enhancing Question-Answering through Automated Ontology Deriv…]]
- [[2025-05-16-arxiv-2505-10900-ikgr-intent-knowledge-graph-recommender|Tuning-Free LLM Can Build A Strong Recommender Under Sparse Connectivi…]]
