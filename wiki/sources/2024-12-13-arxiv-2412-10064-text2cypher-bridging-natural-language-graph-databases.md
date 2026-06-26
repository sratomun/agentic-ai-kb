---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Text2Cypher: Bridging Natural Language and Graph Databases"
authors: Makbule Gulcin Ozsoy et al. (Neo4j)
url: https://arxiv.org/abs/2412.10064
date: 2024-12-13
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, text-to-cypher, semantic-parsing, knowledge-graph]
---

# Text2Cypher: Bridging Natural Language and Graph Databases

**arXiv [2412.10064](https://arxiv.org/abs/2412.10064)** · 2024-12-13 · Neo4j

**Significance.** The dataset that made text-to-Cypher a tractable benchmark task — the field's BIRD/Spider moment for graphs. Anchor for [[text-to-cypher]].

## Abstract
Translating NL to Cypher (graph databases) has lagged text-to-SQL despite graph databases' growing use. Neo4j consolidates a standardized 44,387-instance Text2Cypher dataset, benchmarks foundational and fine-tuned LLMs, and shows fine-tuning helps.

## From the paper (full-text)
**Contribution / method.** Unifies Cypher resources, synthetic, crowdsourced, and prior datasets into **44,387 instances** (NL question + schema + Cypher + provenance), split **39,554 train / 4,833 test** with matched source distributions. Benchmarks closed (GPT-4o, Gemini), open (Llama-3, CodeGemma), and prior fine-tuned models on **Google-BLEU**, **Exact-Match**, and execution-based evaluation; models get question+schema and are constrained to schema-only Cypher output.
**Results.** Closed foundational models (GPT-4o, Gemini) performed best out of the box. Fine-tuning on the training set improved **Google-BLEU by 0.13-0.34** and **Exact-Match by 0.01-0.11** across model families — lifting weaker open models substantially. Limitations flagged: paraphrase sensitivity, schema complexity, and that syntactic correctness ≠ correct results (execution eval still thin).
**Takeaway.** Like text-to-SQL, the bottleneck was data; a standardized corpus + fine-tuning closes most of the gap. Sets up the synthetic-data and schema-filtering work that follows.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing]] · [[knowledge-graph]]
- **Entities:** [[cypher]] · [[neo4j]] · [[text2cypher-dataset]]
- **Raw:** full-text report (alphaXiv) read 2026-06-23
