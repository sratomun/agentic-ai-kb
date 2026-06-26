---
type: source
source_type: arxiv
title: "EPM-RL: Reinforcement Learning for On-Premise Product Mapping in E-Commerce"
authors: Minhyeong Yu, Wonduk Seo
url: https://arxiv.org/abs/2604.23993v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agent-economies, agent-reliability, agentic-rl, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# EPM-RL: Reinforcement Learning for On-Premise Product Mapping in E-Commerce

**arXiv:** [2604.23993v1](https://arxiv.org/abs/2604.23993v1) · 2026-04-27 · cs.CL
**Authors:** Minhyeong Yu, Wonduk Seo

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Product mapping, the task of deciding whether two e-commerce listings refer to the same product, is a core problem for price monitoring and channel visibility. In real marketplaces, however, sellers frequently inject promotional keywords, platform-specific tags, and bundle descriptions into titles, causing the same product to appear under many different names. Recent LLM-based and multi-agent frameworks improve robustness and interpretability on such hard cases, but they often rely on expensive external APIs, repeated retrieval, and complex inference-time orchestration, making large-scale deployment costly and difficult in privacy-sensitive enterprise settings. To address these issues, we present EPM-RL, a reinforcement-learning-based framework for building an accurate and efficient on-premise e-commerce product mapping model. Our central idea is to distill high-cost agentic reasoning into a trainable in-house model. Starting from a curated set of product pairs with LLM-generated rationales and human verification, we first perform parameter-efficient fine-tuning (PEFT) on a small student model using structured reasoning outputs. We then further optimize the model with Reinforcement Learning (RL) using an agent-based reward that jointly evaluates output-format compliance, label correctness, reasoning--preference scores from specially designed judge models. Preliminary results show that EPM-RL consistently improves over PEFT-only training and offers a stronger quality--cost trade-off than commercial API-based baselines, while enabling private deployment and lower operational cost. These findings suggest that reinforcement learning can turn product mapping from a high-latency agentic pipeline into a scalable, inspectable, and production-ready in-house system.

## Graph
- **Concepts:** [[agent-economies|Agent economies]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23993v1)
