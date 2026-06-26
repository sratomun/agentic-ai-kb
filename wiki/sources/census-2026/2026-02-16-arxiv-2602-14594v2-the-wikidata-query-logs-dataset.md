---
type: source
source_type: arxiv
title: "The Wikidata Query Logs Dataset"
authors: Sebastian Walter, Hannah Bast
url: https://arxiv.org/abs/2602.14594v2
date: 2026-02-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 0
primary: cs.CL
tags: [knowledge-graph, arxiv, auto-ingested]
---

# The Wikidata Query Logs Dataset

**arXiv:** [2602.14594v2](https://arxiv.org/abs/2602.14594v2) · 2026-02-16 · cs.CL
**Authors:** Sebastian Walter, Hannah Bast

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present the Wikidata Query Logs (WDQL) dataset, a dataset consisting of 335k question-query pairs over the Wikidata knowledge graph. It is over 11x larger than the largest existing Wikidata datasets of similar format without relying on template-generated queries. Instead, we construct it using real-world SPARQL queries sent to the Wikidata Query Service and generate questions for them. Since these log-based queries are anonymized, and therefore often do not produce results, a significant amount of effort is needed to convert them back into meaningful SPARQL queries. To achieve this, we present an agent-based method that iteratively de-anonymizes, cleans, and verifies queries against Wikidata while also generating corresponding natural-language questions. We demonstrate the benefit of this dataset for training question-answering methods. All WDQL assets, as well as the agent code, are publicly available via https://github.com/ad-freiburg/wikidata-query-logs under a permissive license.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14594v2)
