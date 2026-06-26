---
type: source
source_type: arxiv
title: "NOEM$^{3}$A: A Neuro-Symbolic Ontology-Enhanced Method for Multi-Intent Understanding in Mobile Agents"
authors: Ioannis Tzachristas, Aifen Sui
url: https://arxiv.org/abs/2511.19780v1
date: 2025-11-24
depth: abstract
auto: true
score: 6
primary: cs.AI
tags: [intent-understanding, knowledge-graph, arxiv, auto-ingested]
---

# NOEM$^{3}$A: A Neuro-Symbolic Ontology-Enhanced Method for Multi-Intent Understanding in Mobile Agents

**arXiv:** [2511.19780v1](https://arxiv.org/abs/2511.19780v1) · 2025-11-24 · cs.AI
**Authors:** Ioannis Tzachristas, Aifen Sui

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
We introduce a neuro-symbolic framework for multi-intent understanding in mobile AI agents by integrating a structured intent ontology with compact language models. Our method leverages retrieval-augmented prompting, logit biasing and optional classification heads to inject symbolic intent structure into both input and output representations. We formalize a new evaluation metric-Semantic Intent Similarity (SIS)-based on hierarchical ontology depth, capturing semantic proximity even when predicted intents differ lexically. Experiments on a subset of ambiguous/demanding dialogues of MultiWOZ 2.3 (with oracle labels from GPT-o3) demonstrate that a 3B Llama model with ontology augmentation approaches GPT-4 accuracy (85% vs 90%) at a tiny fraction of the energy and memory footprint. Qualitative comparisons show that ontology-augmented models produce more grounded, disambiguated multi-intent interpretations. Our results validate symbolic alignment as an effective strategy for enabling accurate and efficient on-device NLU.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[knowledge-graph|Knowledge graph]]
- **Entities:** [[multiwoz]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.19780v1)
