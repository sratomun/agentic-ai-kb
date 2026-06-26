---
type: source
source_type: arxiv
title: "Open Biomedical Knowledge Graphs at Scale: Construction, Federation, and AI Agent Access with Samyama Graph Database"
authors: Madhulatha Mandarapu, Sandeep Kunkunuru
url: https://arxiv.org/abs/2603.15080v3
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.DB
tags: [clinical-agents, knowledge-graph, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# Open Biomedical Knowledge Graphs at Scale: Construction, Federation, and AI Agent Access with Samyama Graph Database

**arXiv:** [2603.15080v3](https://arxiv.org/abs/2603.15080v3) · 2026-03-16 · cs.DB
**Authors:** Madhulatha Mandarapu, Sandeep Kunkunuru

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Biomedical knowledge is fragmented across siloed databases -- Reactome for pathways, STRING for protein interactions, ClinicalTrials.gov for study registries, DrugBank for drug vocabularies, DGIdb for drug-gene interactions, SIDER for side effects. We present three open-source biomedical knowledge graphs -- Pathways KG (118,686 nodes, 834,785 edges from 5 sources), Clinical Trials KG (7,774,446 nodes, 26,973,997 edges from 5 sources), and Drug Interactions KG (32,726 nodes, 191,970 edges from 3 sources) -- built on Samyama, a high-performance graph database written in Rust. Our contributions are threefold. First, we describe a reproducible ETL pattern for constructing large-scale KGs from heterogeneous public data sources, with cross-source deduplication, batch loading (Python Cypher and Rust native loaders), and portable snapshot export. Second, we demonstrate cross-KG federation: loading all three snapshots into a single graph tenant enables property-based joins across datasets. Third, we introduce schema-driven MCP server generation for LLM agent access, evaluated on a new BiomedQA benchmark (40 pharmacology questions): domain-specific MCP tools achieve 98% accuracy vs. 85% for schema-aware text-to-Cypher and 75% for standalone GPT-4o, with zero schema errors. All data sources are open-license. The combined federated graph (7.9M nodes, 28M edges) loads in approximately 3 minutes on commodity cloud hardware, with single-KG queries completing in 80-100ms and cross-KG federation joins in 1-4s

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]] · [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.15080v3)
