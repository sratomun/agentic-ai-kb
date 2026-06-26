---
type: source
source_type: arxiv
title: "The Science Data Lake: A Unified Open Infrastructure Integrating 293 Million Papers Across Eight Scholarly Sources with Embedding-Based Ontology Alignment"
authors: Jonas Wilinski
url: https://arxiv.org/abs/2603.03126v1
date: 2026-03-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.DL
tags: [recommendation-agents, science-agents, knowledge-graph, arxiv, auto-ingested]
---

# The Science Data Lake: A Unified Open Infrastructure Integrating 293 Million Papers Across Eight Scholarly Sources with Embedding-Based Ontology Alignment

**arXiv:** [2603.03126v1](https://arxiv.org/abs/2603.03126v1) · 2026-03-03 · cs.DL
**Authors:** Jonas Wilinski

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Scholarly data are largely fragmented across siloed databases with divergent metadata and missing linkages among them. We present the Science Data Lake, a locally-deployable infrastructure built on DuckDB and simple Parquet files that unifies eight open sources - Semantic Scholar, OpenAlex, SciSciNet, Papers with Code, Retraction Watch, Reliance on Science, a preprint-to-published mapping, and Crossref - via DOI normalization while preserving source-level schemas. The resource comprises approximately 960GB of Parquet files spanning ~293 million uniquely identifiable papers across ~22 schemas and ~153 SQL views. An embedding-based ontology alignment using BGE-large sentence embeddings maps 4,516 OpenAlex topics to 13 scientific ontologies (~1.3 million terms), yielding 16,150 mappings covering 99.8% of topics ($\geq 0.65$ threshold) with $F1 = 0.77$ at the recommended $\geq 0.85$ operating point, outperforming TF-IDF, BM25, and Jaro-Winkler baselines on a 300-pair gold-standard evaluation. We validate through 10 automated checks, cross-source citation agreement analysis (pairwise Pearson $r = 0.76$ - $0.87$), and stratified manual annotation. Four vignettes demonstrate cross-source analyses infeasible with any single database. The resource is open source, deployable on a single drive or queryable remotely via HuggingFace, and includes structured documentation suitable for large language model (LLM) based research agents.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.03126v1)
