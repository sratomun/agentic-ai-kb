---
type: source
source_type: arxiv
title: "Neuro-Oracle: A Trajectory-Aware Agentic RAG Framework for Interpretable Epilepsy Surgical Prognosis"
authors: Aizierjiang Aiersilan, Mohamad Koubeissi
url: https://arxiv.org/abs/2604.14216v1
date: 2026-04-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MM
tags: [clinical-agents, agent-protocols, agentic-rag, governance-gap, arxiv, auto-ingested]
---

# Neuro-Oracle: A Trajectory-Aware Agentic RAG Framework for Interpretable Epilepsy Surgical Prognosis

**arXiv:** [2604.14216v1](https://arxiv.org/abs/2604.14216v1) · 2026-04-10 · cs.MM
**Authors:** Aizierjiang Aiersilan, Mohamad Koubeissi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Predicting post-surgical seizure outcomes in pharmacoresistant epilepsy is a clinical challenge. Conventional deep-learning approaches operate on static, single-timepoint pre-operative scans, omitting longitudinal morphological changes. We propose \emph{Neuro-Oracle}, a three-stage framework that: (i) distils pre-to-post-operative MRI changes into a compact 512-dimensional trajectory vector using a 3D Siamese contrastive encoder; (ii) retrieves historically similar surgical trajectories from a population archive via nearest-neighbour search; and (iii) synthesises a natural-language prognosis grounded in the retrieved evidence using a quantized Llama-3-8B reasoning agent. Evaluations are conducted on the public EPISURG dataset ($N{=}268$ longitudinally paired cases) using five-fold stratified cross-validation. Since ground-truth seizure-freedom scores are unavailable, we utilize a clinical proxy label based on the resection type. We acknowledge that the network representations may potentially learn the anatomical features of the resection cavities (i.e., temporal versus non-temporal locations) rather than true prognostic morphometry. Our current evaluation thus serves mainly as a proof-of-concept for the trajectory-aware retrieval architecture. Trajectory-based classifiers achieve AUC values between 0.834 and 0.905, compared with 0.793 for a single-timepoint ResNet-50 baseline. The Neuro-Oracle agent (M5) matches the AUC of purely discriminative trajectory classifiers (0.867) while producing structured justifications with zero observed hallucinations under our audit protocol. A Siamese Diversity Ensemble (M6) of trajectory-space classifiers attains an AUC of 0.905 without language-model overhead.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-protocols|Agent protocols]] · [[agentic-rag|Agentic RAG]] · [[governance-gap|Governance gap]]
- **Entities:** [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14216v1)
