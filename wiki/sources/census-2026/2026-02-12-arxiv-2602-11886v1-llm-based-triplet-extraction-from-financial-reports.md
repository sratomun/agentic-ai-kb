---
type: source
source_type: arxiv
title: "LLM-based Triplet Extraction from Financial Reports"
authors: Dante Wesslund, Ville Stenström, Pontus Linde, Alexander Holmberg
url: https://arxiv.org/abs/2602.11886v1
date: 2026-02-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 1
primary: cs.CL
tags: [finance-agents, knowledge-graph, arxiv, auto-ingested]
---

# LLM-based Triplet Extraction from Financial Reports

**arXiv:** [2602.11886v1](https://arxiv.org/abs/2602.11886v1) · 2026-02-12 · cs.CL
**Authors:** Dante Wesslund, Ville Stenström, Pontus Linde, Alexander Holmberg

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Corporate financial reports are a valuable source of structured knowledge for Knowledge Graph construction, but the lack of annotated ground truth in this domain makes evaluation difficult. We present a semi-automated pipeline for Subject-Predicate-Object triplet extraction that uses ontology-driven proxy metrics, specifically Ontology Conformance and Faithfulness, instead of ground-truth-based evaluation. We compare a static, manually engineered ontology against a fully automated, document-specific ontology induction approach across different LLMs and two corporate annual reports. The automatically induced ontology achieves 100% schema conformance in all configurations, eliminating the ontology drift observed with the manual approach. We also propose a hybrid verification strategy that combines regex matching with an LLM-as-a-judge check, reducing apparent subject hallucination rates from 65.2% to 1.6% by filtering false positives caused by coreference resolution. Finally, we identify a systematic asymmetry between subject and object hallucinations, which we attribute to passive constructions and omitted agents in financial prose.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.11886v1)
