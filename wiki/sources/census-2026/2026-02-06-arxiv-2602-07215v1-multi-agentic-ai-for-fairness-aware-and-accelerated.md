---
type: source
source_type: arxiv
title: "Multi-Agentic AI for Fairness-Aware and Accelerated Multi-modal Large Model Inference in Real-world Mobile Edge Networks"
authors: Haiyuan Li, Hari Madhukumar, Shuangyi Yan, Yulei Wu et al.
url: https://arxiv.org/abs/2602.07215v1
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: eess.SY
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Agentic AI for Fairness-Aware and Accelerated Multi-modal Large Model Inference in Real-world Mobile Edge Networks

**arXiv:** [2602.07215v1](https://arxiv.org/abs/2602.07215v1) · 2026-02-06 · eess.SY
**Authors:** Haiyuan Li, Hari Madhukumar, Shuangyi Yan, Yulei Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generative AI (GenAI) has transformed applications in natural language processing and content creation, yet centralized inference remains hindered by high latency, limited customizability, and privacy concerns. Deploying large models (LMs) in mobile edge networks emerges as a promising solution. However, it also poses new challenges, including heterogeneous multi-modal LMs with diverse resource demands and inference speeds, varied prompt/output modalities that complicate orchestration, and resource-limited infrastructure ill-suited for concurrent LM execution. In response, we propose a Multi-Agentic AI framework for latency- and fairness-aware multi-modal LM inference in mobile edge networks. Our solution includes a long-term planning agent, a short-term prompt scheduling agent, and multiple on-node LM deployment agents, all powered by foundation language models. These agents cooperatively optimize prompt routing and LM deployment through natural language reasoning over runtime telemetry and historical experience. To evaluate its performance, we further develop a city-wide testbed that supports network monitoring, containerized LM deployment, intra-server resource management, and inter-server communications. Experiments demonstrate that our solution reduces average latency by over 80% and improves fairness (Normalized Jain index) to 0.90 compared to other baselines. Moreover, our solution adapts quickly without fine-tuning, offering a generalizable solution for optimizing GenAI services in edge environments.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.07215v1)
