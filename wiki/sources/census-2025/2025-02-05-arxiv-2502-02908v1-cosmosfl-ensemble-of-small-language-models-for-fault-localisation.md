---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "COSMosFL: Ensemble of Small Language Models for Fault Localisation"
authors: Hyunjoon Cho et al.
url: https://arxiv.org/abs/2502.02908v1
date: 2025-02-05
score: 1
primary: cs.SE
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, coding-agents, clinical-agents]
---

# COSMosFL: Ensemble of Small Language Models for Fault Localisation

**arXiv:** [2502.02908v1](https://arxiv.org/abs/2502.02908v1) · 2025-02-05 · cs.SE
**Authors:** Hyunjoon Cho et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLMs are rapidly being adopted to build powerful tools and agents for software engineering, but most of them rely heavily on extremely large closed-source models. This, in turn, can hinder wider adoption due to security issues as well as financial cost and environmental impact. Recently, a number of open source Small Language Models (SLMs) are being released and gaining traction. While SLMs are smaller, more energy-efficient, and therefore easier to locally deploy, they tend to show worse performance when compared to larger closed LLMs. We present COSMos, a task-level LLM ensemble technique that uses voting mechanism, to provide a broader range of choice between SLMs and LLMs. We instantiate COSMos with an LLM-based Fault Localisation technique, AutoFL, and report the cost-benefit trade-off between LLM accuracy and various costs such as energy consumption, inference time, and the number of tokens used. An empirical evaluation using Defects4J shows that COSMos can build effective ensembles that can achieve Pareto-optimality in terms of FL accuracy and inference cost, when compared to individual models.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[coding-agents]] · [[clinical-agents]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2502.02908v1)
