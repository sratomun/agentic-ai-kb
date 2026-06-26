---
type: source
source_type: arxiv
title: "EviSearch: A Human in the Loop System for Extracting and Auditing Clinical Evidence for Systematic Reviews"
authors: Naman Ahuja, Saniya Mulla, Muhammad Ali Khan, Zaryab Bin Riaz et al.
url: https://arxiv.org/abs/2604.14165v2
date: 2026-03-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.CL
tags: [clinical-agents, knowledge-graph, human-agent-interaction, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# EviSearch: A Human in the Loop System for Extracting and Auditing Clinical Evidence for Systematic Reviews

**arXiv:** [2604.14165v2](https://arxiv.org/abs/2604.14165v2) · 2026-03-23 · cs.CL
**Authors:** Naman Ahuja, Saniya Mulla, Muhammad Ali Khan, Zaryab Bin Riaz et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present EviSearch, a multi-agent extraction system that automates the creation of ontology-aligned clinical evidence tables directly from native trial PDFs while guaranteeing per-cell provenance for audit and human verification. EviSearch pairs a PDF-query agent (which preserves rendered layout and figures) with a retrieval-guided search agent and a reconciliation module that forces page-level verification when agents disagree. The pipeline is designed for high-precision extraction across multimodal evidence sources (text, tables, figures) and for generating reviewer-actionable provenance that clinicians can inspect and correct. On a clinician-curated benchmark of oncology trial papers, EviSearch substantially improves extraction accuracy relative to strong parsed-text baselines while providing comprehensive attribution coverage. By logging reconciler decisions and reviewer edits, the system produces structured preference and supervision signals that bootstrap iterative model improvement. EviSearch is intended to accelerate living systematic review workflows, reduce manual curation burden, and provide a safe, auditable path for integrating LLM-based extraction into evidence synthesis pipelines.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[human-agent-interaction|Human-agent interaction]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14165v2)
