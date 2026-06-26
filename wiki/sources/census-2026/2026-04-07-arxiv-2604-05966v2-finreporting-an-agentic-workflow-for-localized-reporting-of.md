---
type: source
source_type: arxiv
title: "FinReporting: An Agentic Workflow for Localized Reporting of Cross-Jurisdiction Financial Disclosures"
authors: Fan Zhang, Mingzi Song, Rania Elbadry, Yankai Chen et al.
url: https://arxiv.org/abs/2604.05966v2
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.CL
tags: [finance-agents, knowledge-graph, agent-reliability, governance-gap, arxiv, auto-ingested]
---

# FinReporting: An Agentic Workflow for Localized Reporting of Cross-Jurisdiction Financial Disclosures

**arXiv:** [2604.05966v2](https://arxiv.org/abs/2604.05966v2) · 2026-04-07 · cs.CL
**Authors:** Fan Zhang, Mingzi Song, Rania Elbadry, Yankai Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Financial reporting systems increasingly leverage Large Language Models (LLMs) to extract and summarize corporate disclosures. However, most existing approaches assume a single-market setting and overlook structural differences across jurisdictions. Variations in accounting taxonomies, tagging infrastructures (e.g., XBRL vs.\ PDF), and aggregation conventions introduce substantial challenges for semantic alignment and reliable verification. Here, we aim to bridge this gap. We present FinReporting, an agentic workflow for localized cross-jurisdiction financial reporting. The system constructs a unified canonical ontology spanning the income statement, balance sheet, and cash flow statement, and decomposes reporting into auditable stages, including filing acquisition, extraction, canonical mapping, and anomaly logging. Rather than treating LLMs as free-form generators, FinReporting employs them as constrained verifiers operating under explicit decision rules with evidence grounding. Evaluated on annual filings from the USA, Japan, and China, FinReporting improves consistency and reliability under heterogeneous reporting regimes. We further release an interactive demo that enables cross-market inspection and supports structured export of localized financial statements. Our demo is available at url{https://huggingface.co/spaces/BoomQ/FinReporting-Demo. A video describing our system is available at https://www.youtube.com/watch?v=f65jdEL31Kk.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05966v2)
