---
type: source
source_type: arxiv
title: "TimeART: Towards Agentic Time Series Reasoning via Tool-Augmentation"
authors: Xingjian Wu, Junkai Lu, Zhengyu Li, Xiangfei Qiu et al.
url: https://arxiv.org/abs/2601.13653v1
date: 2026-01-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.LG
tags: [finance-agents, tool-use, arxiv, auto-ingested]
---

# TimeART: Towards Agentic Time Series Reasoning via Tool-Augmentation

**arXiv:** [2601.13653v1](https://arxiv.org/abs/2601.13653v1) · 2026-01-20 · cs.LG
**Authors:** Xingjian Wu, Junkai Lu, Zhengyu Li, Xiangfei Qiu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Time series data widely exist in real-world cyber-physical systems. Though analyzing and interpreting them contributes to significant values, e.g, disaster prediction and financial risk control, current workflows mainly rely on human data scientists, which requires significant labor costs and lacks automation. To tackle this, we introduce TimeART, a framework fusing the analytical capability of strong out-of-the-box tools and the reasoning capability of Large Language Models (LLMs), which serves as a fully agentic data scientist for Time Series Question Answering (TSQA). To teach the LLM-based Time Series Reasoning Models (TSRMs) strategic tool-use, we also collect a 100k expert trajectory corpus called TimeToolBench. To enhance TSRMs' generalization capability, we then devise a four-stage training strategy, which boosts TSRMs through learning from their own early experiences and self-reflections. Experimentally, we train an 8B TSRM on TimeToolBench and equip it with the TimeART framework, and it achieves consistent state-of-the-art performance on multiple TSQA tasks, which pioneers a novel approach towards agentic time series reasoning.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[tool-use|Tool use]]
- **Entities:** [[toolbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.13653v1)
