---
type: concept
tags: [agents, semantic-parsing, text-to-sql, text-to-cypher, nlu]
created: 2026-06-23
updated: 2026-06-23
kind: hub
---

# Semantic parsing

*Translating natural-language intent into an executable structured query or logical form — the parent task whose children differ only by target formalism (SQL, Cypher, SPARQL).*

## What it is
The task of mapping an utterance to an executable meaning representation against a schema. Its children are formalism-specific: **[[text-to-sql]]** (relational tables/joins), **[[text-to-cypher]]** (property-graph nodes/edges/paths), and SPARQL (RDF triples). They share the same hard sub-problems — schema linking, ambiguity resolution, and execution-guided correctness — and, crucially, **transfer**: training on one formalism improves another.

## Why it matters
This is the executable end of [[intent-understanding]] and the engine under [[intent-grounding]]: once intent is resolved against a structure, semantic parsing is what turns it into a runnable query. For the exec the practical point is that SQL and Cypher are *one capability with two outputs* — a metrics/semantic-layer vault and a knowledge-graph (`sem:lineage`) are queried by the same parsing skill, so investment compounds across both. The clearest proof: a single model jointly trained on SQL and Cypher transfers across them — **Spider +13.5% and Text2Cypher +73.1%** even without shared schemas ([[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM]]).

## What the evidence shows
**Foundations — the shared sub-problems.** Every formalism fights the same three battles. **Schema linking** (which tables/labels/relations does the question touch?) dominates cost and accuracy: filtering the schema to the relevant slice cuts prompt size ~6× and roughly halves cost while *raising* small-model accuracy ([[2025-05-08-arxiv-2505-05118-enhancing-text2cypher-with-schema-filtering|Schema Filtering]]). **Ambiguity** persists even with the schema in context — scope, attachment, vagueness — and frontier models miss it ([[2024-06-27-arxiv-2406-19073-ambrosia-parsing-ambiguous-questions|AMBROSIA]]); the fix is disambiguate-in-NL-then-parse ([[2025-02-25-arxiv-2502-18448-disambiguate-first-parse-later|Disambiguate First, Parse Later]]). **Execution is signal, not just validation:** keep grounding open until the database disambiguates it ([[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|GATE]]); feed execution errors back via in-context learning to cut execution-error rate 41-50% ([[2026-05-21-arxiv-2605-22937-ras-reflection-augmented-scaling-cypher|RAS]]).

**Recent developments — convergence and unification.** The field is unifying across formalisms: STRuCT-LLM trains SQL+Cypher jointly with cross-transfer; UniQGen generates intent-aligned queries across query languages without schema-matching fine-tuning (**+31.6% F1 on GraphQ**, [[2026-04-09-arxiv-2605-00845-uniqgen-constraint-guided-graph-query-generation|UniQGen]]); and unified benchmarks now span many graph dialects — **178,184 pairs across 13 domains**, exposing a brutal ISO-GQL gap (≤4% zero-shot execution accuracy → 45.1% fine-tuned) ([[2026-02-12-arxiv-2602-11745-text2gql-bench|Text2GQL-Bench]]). The throughline: **exposure to enough formalism-specific examples is what unlocks accuracy**, and synthetic data is how that gap gets closed.

## Includes (children)
- [[text-to-sql]] — relational target (the existing [[data-query-agents]] node is its *agentic application*)
- [[text-to-cypher]] — property-graph target
- (SPARQL / RDF — folded here for now; promote if the corpus grows)

## Relationships
- executable end of [[intent-understanding]]; engine of [[intent-grounding]]
- children: [[text-to-sql]] · [[text-to-cypher]]
- applied by [[data-query-agents]]
- the wrappers in [[mediated-semantic-architecture]] (via [[text-to-query-wrapper]])
- targets: [[metrics-layer]] (relational) · [[knowledge-graph]] (graph)
- shared challenge with the clarification/disambiguation thread in [[intent-understanding]]

## Key papers (curated by relevance)
<!-- Curated from the papers this node cites + backlinks; per-paper citation counts not in the 2025–26 census window. Ordered by velocity/recency. -->
- [[2026-06-12-arxiv-2606-14325-precise-text-to-cypher-grounded-kg-data-generation|Achieving Precise Text-To-Cypher Via Grounded Knowledge Graph Data Gen…]]
- [[2026-06-04-arxiv-2606-05634-bootstrapping-semantic-layer-from-execution-text-to-sql|Bootstrapping Semantic Layer from Execution for Text-to-SQL]]
- [[2026-05-28-arxiv-2605-29250-omniretrieval-unified-retrieval-heterogeneous|OmniRetrieval: Unified Retrieval across Heterogeneous Knowledge Source…]]
- [[2026-05-21-arxiv-2605-22937-ras-reflection-augmented-scaling-cypher|RAS: Reflection-Augmented Scaling with In-Context Learning for Executa…]]
- [[2026-04-09-arxiv-2605-00845-uniqgen-constraint-guided-graph-query-generation|Graph Query Generation with Constraint-guided Large Language Agents (U…]]
- [[2026-02-12-arxiv-2602-11745-text2gql-bench|Text2GQL-Bench: A Text to Graph Query Language Benchmark]]
- [[2025-10-18-arxiv-2510-16470-declarative-nl-queries-over-heterogeneous-data|Declarative Techniques for NL Queries over Heterogeneous Data]]
- [[2025-06-15-arxiv-2506-21575-struct-llm-tabular-graph-semantic-parsing|STRuCT-LLM: Unifying Tabular and Graph Reasoning with Reinforcement Le…]]
- [[2025-05-08-arxiv-2505-05118-enhancing-text2cypher-with-schema-filtering|Enhancing Text2Cypher with Schema Filtering]]
