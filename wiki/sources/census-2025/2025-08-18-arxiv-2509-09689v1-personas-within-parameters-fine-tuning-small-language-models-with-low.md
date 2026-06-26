---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Personas within Parameters: Fine-Tuning Small Language Models with Low-Rank Adapters to Mimic User Behaviors"
authors: Himanshu Thakur et al.
url: https://arxiv.org/abs/2509.09689v1
date: 2025-08-18
score: -2
primary: cs.IR
tags: [arxiv, auto-ingested, small-language-models, post-training, recommendation-agents]
---

# Personas within Parameters: Fine-Tuning Small Language Models with Low-Rank Adapters to Mimic User Behaviors

**arXiv:** [2509.09689v1](https://arxiv.org/abs/2509.09689v1) · 2025-08-18 · cs.IR
**Authors:** Himanshu Thakur et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
A long-standing challenge in developing accurate recommendation models is simulating user behavior, mainly due to the complex and stochastic nature of user interactions. Towards this, one promising line of work has been the use of Large Language Models (LLMs) for simulating user behavior. However, aligning these general-purpose large pre-trained models with user preferences necessitates: (i) effectively and continously parsing large-scale tabular user-item interaction data, (ii) overcoming pre-training-induced inductive biases to accurately learn user specific knowledge, and (iii) achieving the former two at scale for millions of users. While most previous works have focused on complex methods to prompt an LLM or fine-tune it on tabular interaction datasets, our approach shifts the focus to extracting robust textual user representations using a frozen LLM and simulating cost-effective, resource-efficient user agents powered by fine-tuned Small Language Models (SLMs). Further, we showcase a method for training multiple low-rank adapters for groups of users or \textit{persona}, striking an optimal balance between scalability and performance of user behavior agents. Our experiments provide compelling empirical evidence of the efficacy of our methods, demonstrating that user agents developed using our approach have the potential to bridge the gap between offline metrics and real-world performance of recommender systems.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[post-training]] · [[recommendation-agents]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2509.09689v1)
