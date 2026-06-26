---
type: source
source_type: arxiv
title: "MechPert: Mechanistic Consensus as an Inductive Bias for Unseen Perturbation Prediction"
authors: Marc Boubnovski Martell, Josefa Lia Stoisser, Lawrence Phillips, Aditya Misra et al.
url: https://arxiv.org/abs/2602.13791v1
date: 2026-02-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.LG
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# MechPert: Mechanistic Consensus as an Inductive Bias for Unseen Perturbation Prediction

**arXiv:** [2602.13791v1](https://arxiv.org/abs/2602.13791v1) · 2026-02-14 · cs.LG
**Authors:** Marc Boubnovski Martell, Josefa Lia Stoisser, Lawrence Phillips, Aditya Misra et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Predicting transcriptional responses to unseen genetic perturbations is essential for understanding gene regulation and prioritizing large-scale perturbation experiments. Existing approaches either rely on static, potentially incomplete knowledge graphs, or prompt language models for functionally similar genes, retrieving associations shaped by symmetric co-occurrence in scientific text rather than directed regulatory logic. We introduce MechPert, a lightweight framework that encourages LLM agents to generate directed regulatory hypotheses rather than relying solely on functional similarity. Multiple agents independently propose candidate regulators with associated confidence scores; these are aggregated through a consensus mechanism that filters spurious associations, producing weighted neighborhoods for downstream prediction. We evaluate MechPert on Perturb-seq benchmarks across four human cell lines. For perturbation prediction in low-data regimes ($N=50$ observed perturbations), MechPert improves Pearson correlation by up to 10.5\% over similarity-based baselines. For experimental design, MechPert-selected anchor genes outperform standard network centrality heuristics by up to 46\% in well-characterized cell lines.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13791v1)
