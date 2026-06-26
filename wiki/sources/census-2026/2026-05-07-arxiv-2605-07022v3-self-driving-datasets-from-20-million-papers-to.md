---
type: source
source_type: arxiv
title: "Self-Driving Datasets: From 20 Million Papers to Nuanced Biomedical Knowledge at Scale"
authors: Haydn Jones, Yimeng Zeng, Alden Rose, Li S. Yifei et al.
url: https://arxiv.org/abs/2605.07022v3
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.LG
tags: [autonomous-driving-agents, science-agents, knowledge-graph, multi-agent-systems, arxiv, auto-ingested]
---

# Self-Driving Datasets: From 20 Million Papers to Nuanced Biomedical Knowledge at Scale

**arXiv:** [2605.07022v3](https://arxiv.org/abs/2605.07022v3) · 2026-05-07 · cs.LG
**Authors:** Haydn Jones, Yimeng Zeng, Alden Rose, Li S. Yifei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Manually curated biomedical repositories -- spanning bioactivity, genomics, and chemistry -- are expensive to maintain, lag behind primary literature, and discard experimental context, obscuring nuances needed to assess data correctness and coverage. We show that PubMed itself can be autonomously and cost-effectively turned into structured datasets that are larger, more nuanced, and more accurate than the curated databases they replace. We present three coupled contributions: (1) an LLM-based entity-tagging pipeline, grounded in nine biomedical ontologies, that tags 4.5B entities across 19 categories in a 22.5M-paper, 2.5T-token PubMed corpus; (2) hybrid sparse-dense retrieval supporting entity-filtered semantic queries over the tagged corpus; and (3) Starling, a multi-agent deep research system that, given only a natural-language task description, designs precision- and recall-targeted retrieval filters, induces an extraction schema, and emits structured records with nuance-rich fields and supporting passages. Across six tasks -- blood-brain barrier permeability, oral bioavailability, acute toxicity (LD50), gene-disease associations, protein subcellular localization, and chemical reactions -- Starling produces ~6.3M records (91K-3M per task); several are, to our knowledge, the largest public datasets for their property. Frontier-model rejection of our extractions is 0.6-7.7% across tasks, far below error rates we measure on widely used curated counterparts (e.g., 16.5% on BBB_Martins, 7.3% on Bioavailability_Ma). Beyond scale and accuracy, the supporting passages carry nuance tabular databases discard -- e.g., oral bioavailability may depend on fed vs. fasted state. Together, the corpus, retrieval, and agent establish a foundation for AI-driven therapeutic design. Code and datasets: https://github.com/starling-labs/starling.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.07022v3)
