---
type: source
source_type: arxiv
title: "AgriWorld:A World Tools Protocol Framework for Verifiable Agricultural Reasoning with Code-Executing LLM Agents"
authors: Zhixing Zhang, Jesen Zhang, Hao Liu, Qinhan Lv et al.
url: https://arxiv.org/abs/2602.15325v1
date: 2026-02-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agent-reliability, agent-protocols, tool-use, arxiv, auto-ingested]
---

# AgriWorld:A World Tools Protocol Framework for Verifiable Agricultural Reasoning with Code-Executing LLM Agents

**arXiv:** [2602.15325v1](https://arxiv.org/abs/2602.15325v1) · 2026-02-17 · cs.AI
**Authors:** Zhixing Zhang, Jesen Zhang, Hao Liu, Qinhan Lv et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Foundation models for agriculture are increasingly trained on massive spatiotemporal data (e.g., multi-spectral remote sensing, soil grids, and field-level management logs) and achieve strong performance on forecasting and monitoring. However, these models lack language-based reasoning and interactive capabilities, limiting their usefulness in real-world agronomic workflows. Meanwhile, large language models (LLMs) excel at interpreting and generating text, but cannot directly reason over high-dimensional, heterogeneous agricultural datasets. We bridge this gap with an agentic framework for agricultural science. It provides a Python execution environment, AgriWorld, exposing unified tools for geospatial queries over field parcels, remote-sensing time-series analytics, crop growth simulation, and task-specific predictors (e.g., yield, stress, and disease risk). On top of this environment, we design a multi-turn LLM agent, Agro-Reflective, that iteratively writes code, observes execution results, and refines its analysis via an execute-observe-refine loop. We introduce AgroBench, with scalable data generation for diverse agricultural QA spanning lookups, forecasting, anomaly detection, and counterfactual "what-if" analysis. Experiments outperform text-only and direct tool-use baselines, validating execution-driven reflection for reliable agricultural reasoning.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.15325v1)
