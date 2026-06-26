---
type: concept
tags: [agents, text-to-cypher, semantic-parsing, knowledge-graph]
created: 2026-06-23
updated: 2026-06-23
kind: domain
---

# Text-to-Cypher

*Translating natural language into Cypher queries over property graphs — the graph sibling of [[text-to-sql]], under [[semantic-parsing]].*

## What it is
Generating executable Cypher (Neo4j's graph query language) from a question plus a graph schema, so non-experts can query property graphs by pattern-matching nodes, relationships, and paths. It is one child of [[semantic-parsing]]; what differs from [[text-to-sql]] is the target formalism — traversal and path patterns rather than joins.

## Why it matters
It's the natural-language front door to a [[knowledge-graph]] — directly relevant to graph-shaped semantic layers and lineage. The headline finding is the same efficiency story as the rest of the intent stack: **graph-grounded synthetic data lets tiny on-prem models rival frontier proprietary systems**, which matters when the graph holds private/governed data you can't send to a closed API.

## What the evidence shows
**Foundations — the data problem and the dataset.** Text-to-Cypher lagged text-to-SQL mainly for lack of data. Neo4j's **Text2Cypher** consolidated 44,387 NL-question/Cypher/schema instances (39,554 train / 4,833 test); off-the-shelf, closed models (GPT-4o, Gemini) led, and fine-tuning lifted Google-BLEU 0.13-0.34 and ExactMatch 0.01-0.11 ([[2024-12-13-arxiv-2412-10064-text2cypher-bridging-natural-language-graph-databases|Text2Cypher]]). Synthetic-data pipelines then closed the gap: **SynthCypher** (29.8k instances, LLM-as-database-filler check) gave up to **+40%** on the test split ([[2024-12-17-arxiv-2412-12612-auto-cypher-llm-supervised-generation-verification|Auto-Cypher]]); **SyntheT2C/MedT2C** did the same for medical KGs ([[2024-06-15-arxiv-2406-10710-synthet2c-synthetic-data-text2cypher|SyntheT2C]]).

**Recent developments — precision, schema, execution, scale.**
- **Grounded synthetic data closes the model-size gap:** CYQUARK fine-tuning takes a 4B model from **37.94 → 76.21** execution accuracy (and a 0.8B model to 73.30) — near Claude Opus 4.7 (78.58) and GPT-5.5 (78.52) ([[2026-06-12-arxiv-2606-14325-precise-text-to-cypher-grounded-kg-data-generation|Precise Text-to-Cypher / CYQUARK]]).
- **Schema filtering is the cost lever:** pruning the schema to exact-match elements cuts P95 prompt tokens ~6× (2697→529) and roughly halves cost, while improving small-model accuracy ([[2025-05-08-arxiv-2505-05118-enhancing-text2cypher-with-schema-filtering|Schema Filtering]]).
- **Execution feedback is signal:** conditioning retries on database error messages cuts execution-error rate **41-50%** at n=5 ([[2026-05-21-arxiv-2605-22937-ras-reflection-augmented-scaling-cypher|RAS]]).
- **Realistic deployments need routing across graphs:** multi-database reasoning (route → decompose → integrate) replaces the single-schema assumption ([[2026-05-11-arxiv-2605-10373-multi-database-query-reasoning-text2cypher|Multi-DB Text2Cypher]]); enterprise benchmark generation accounts for governance/terminology variation ([[2026-06-07-arxiv-2606-08481-pipe-cypher-enterprise-benchmark-generation|PIPE-Cypher]]).
- **Benchmarks matured:** **CypherBench** builds property-graph views over Wikidata (11 graphs, 7.8M entities, 10k+ questions) so LLMs can query encyclopedic KGs with Cypher ([[2024-12-24-arxiv-2412-18702-cypherbench-precise-retrieval-knowledge-graphs|CypherBench]], Megagon — same lab as [[2025-08-29-arxiv-2509-04472-recap-rewriting-conversations-intent-understanding|RECAP]]); and Cypher becomes the engine of [[knowledge-graph|GraphRAG]] over labeled property graphs ([[2025-11-11-arxiv-2511-08274-multi-agent-graphrag-text-to-cypher-lpg|Multi-Agent GraphRAG]]).

## Relationships
- child of [[semantic-parsing]]; sibling of [[text-to-sql]]
- queries [[knowledge-graph]] (property graphs); engine for GraphRAG
- realized by [[data-query-agents]]
- query language: [[cypher]]; benchmarks: [[text2cypher-dataset]] · [[cypherbench]]
- vendor: [[neo4j]]

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. Citations from census/source-note frontmatter. -->
- **5** · 0.7/mo · [[2025-11-11-arxiv-2511-08274-multi-agent-graphrag-text-to-cypher-lpg|Multi-Agent GraphRAG: A Text-to-Cypher Framework for Labeled Prope…]]
- **0** · [[2025-05-08-arxiv-2505-05118-enhancing-text2cypher-with-schema-filtering|Enhancing Text2Cypher with Schema Filtering]]
- **0** · [[2024-12-13-arxiv-2412-10064-text2cypher-bridging-natural-language-graph-databases|Text2Cypher: Bridging Natural Language and Graph Databases]]
- **0** · [[2026-06-12-arxiv-2606-14325-precise-text-to-cypher-grounded-kg-data-generation|Achieving Precise Text-To-Cypher Via Grounded Knowledge Graph Data…]]
