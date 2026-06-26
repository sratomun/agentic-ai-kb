---
type: source
source_type: arxiv
title: "Unsupervised Anomaly Detection in Multi-Agent Trajectory Prediction via Transformer-Based Models"
authors: Qing Lyu, Zhe Fu, Alexandre Bayen
url: https://arxiv.org/abs/2601.20367v1
date: 2026-01-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.LG
tags: [autonomous-driving-agents, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# Unsupervised Anomaly Detection in Multi-Agent Trajectory Prediction via Transformer-Based Models

**arXiv:** [2601.20367v1](https://arxiv.org/abs/2601.20367v1) · 2026-01-28 · cs.LG
**Authors:** Qing Lyu, Zhe Fu, Alexandre Bayen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Identifying safety-critical scenarios is essential for autonomous driving, but the rarity of such events makes supervised labeling impractical. Traditional rule-based metrics like Time-to-Collision are too simplistic to capture complex interaction risks, and existing methods lack a systematic way to verify whether statistical anomalies truly reflect physical danger. To address this gap, we propose an unsupervised anomaly detection framework based on a multi-agent Transformer that models normal driving and measures deviations through prediction residuals. A dual evaluation scheme has been proposed to assess both detection stability and physical alignment: Stability is measured using standard ranking metrics in which Kendall Rank Correlation Coefficient captures rank agreement and Jaccard index captures the consistency of the top-K selected items; Physical alignment is assessed through correlations with established Surrogate Safety Measures (SSM). Experiments on the NGSIM dataset demonstrate our framework's effectiveness: We show that the maximum residual aggregator achieves the highest physical alignment while maintaining stability. Furthermore, our framework identifies 388 unique anomalies missed by Time-to-Collision and statistical baselines, capturing subtle multi-agent risks like reactive braking under lateral drift. The detected anomalies are further clustered into four interpretable risk types, offering actionable insights for simulation and testing.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.20367v1)
