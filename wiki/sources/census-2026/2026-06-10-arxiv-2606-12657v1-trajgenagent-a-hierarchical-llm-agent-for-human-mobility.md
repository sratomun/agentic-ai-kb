---
type: source
source_type: arxiv
title: "TrajGenAgent: A Hierarchical LLM Agent for Human Mobility Trajectory Generation"
authors: Siyu Li, Toan Tran, Lingyi Zhao, Khurram Shafique et al.
url: https://arxiv.org/abs/2606.12657v1
date: 2026-06-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# TrajGenAgent: A Hierarchical LLM Agent for Human Mobility Trajectory Generation

**arXiv:** [2606.12657v1](https://arxiv.org/abs/2606.12657v1) · 2026-06-10 · cs.AI
**Authors:** Siyu Li, Toan Tran, Lingyi Zhao, Khurram Shafique et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Human mobility data is important for transportation, urban planning, and epidemic control, but large-scale trajectory collection is often costly and privacy-constrained, motivating realistic synthetic trajectory generation. Existing LLM-based generators typically rely on either prompt engineering, which preserves zero-shot reasoning but lacks fine-grained spatiotemporal grounding, or trajectory-level fine-tuning, which improves statistical precision but incurs substantial computational cost and may weaken general reasoning. We propose TrajGenAgent, a semantic-aware hierarchical LLM-agent framework for human mobility trajectory generation without model fine-tuning. TrajGenAgent uses a two-stage orchestrator-worker design: an LLM first synthesizes an individual- and weekday-conditioned activity chain from historical evidence via in-context learning, and a deterministic workflow then grounds each activity into a complete visit using personalized POI retrieval, distance-aware location selection, kinematics-aware travel-time propagation, and LLM-based duration estimation. To evaluate realism beyond aggregate spatiotemporal statistics, we introduce an anomaly-detection-based evaluation framework using two complementary detectors to assess behavioral and semantic plausibility. Experiments on benchmark and large-scale simulation datasets show that TrajGenAgent improves spatiotemporal fidelity, semantic coherence, and individual-specific behavioral realism over representative neural and LLM-based baselines, while avoiding parameter updates.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.12657v1)
