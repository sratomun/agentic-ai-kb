---
type: source
source_type: arxiv
title: "Frontier LLM-based agents can overcome the ontology curation bottleneck for natural phenotypes"
authors: James P. Balhoff, Hilmar Lapp
url: https://arxiv.org/abs/2605.28965v1
date: 2026-05-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.AI
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# Frontier LLM-based agents can overcome the ontology curation bottleneck for natural phenotypes

**arXiv:** [2605.28965v1](https://arxiv.org/abs/2605.28965v1) · 2026-05-27 · cs.AI
**Authors:** James P. Balhoff, Hilmar Lapp

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Linking free-text phenotype descriptions to ontology terms, typically referred to as phenotype annotation, is essential for the cross-study integration of comparative morphological data. This labor intensive process has heavily relied on highly trained human experts, which makes it challenging to scale and thus a key bottleneck. Dahdul et al. (2018) established a Gold Standard (GS) of Entity-Quality (EQ) annotations across seven phylogenetic studies and used it to evaluate three human curators and the Semantic CharaParser NLP tool with ontology-based semantic similarity metrics; they reported that machine-human consistency was significantly lower than inter-curator (human-human) consistency. Here we revisit that benchmark with five frontier hosted LLMs from Anthropic and OpenAI, each operating as an "agentic curator" within a self-contained workspace that supplies the source publication PDF, the same annotation guide used by the original human curators, the four project ontologies (UBERON, PATO, BSPO, GO), and a validation script. Evaluated against the same Gold Standard, every agent fell within the range of inter-curator variability of the three trained human biocurators of the original study; the best performing agents approached but did not reach the best performing human curator. Agents substantially outperformed Semantic CharaParser on all four metrics.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.28965v1)
