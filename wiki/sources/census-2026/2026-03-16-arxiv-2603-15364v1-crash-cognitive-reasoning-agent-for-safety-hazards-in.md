---
type: source
source_type: arxiv
title: "CRASH: Cognitive Reasoning Agent for Safety Hazards in Autonomous Driving"
authors: Erick Silva, Rehana Yasmin, Ali Shoker
url: https://arxiv.org/abs/2603.15364v1
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [autonomous-driving-agents, agent-reliability, agent-security, arxiv, auto-ingested]
---

# CRASH: Cognitive Reasoning Agent for Safety Hazards in Autonomous Driving

**arXiv:** [2603.15364v1](https://arxiv.org/abs/2603.15364v1) · 2026-03-16 · cs.AI
**Authors:** Erick Silva, Rehana Yasmin, Ali Shoker

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As AVs grow in complexity and diversity, identifying the root causes of operational failures has become increasingly complex. The heterogeneity of system architectures across manufacturers, ranging from end-to-end to modular designs, together with variations in algorithms and integration strategies, limits the standardization of incident investigations and hinders systematic safety analysis. This work examines real-world AV incidents reported in the NHTSA database. We curate a dataset of 2,168 cases reported between 2021 and 2025, representing more than 80 million miles driven. To process this data, we introduce CRASH, Cognitive Reasoning Agent for Safety Hazards, an LLM-based agent that automates reasoning over crash reports by leveraging both standardized fields and unstructured narrative descriptions. CRASH operates on a unified representation of each incident to generate concise summaries, attribute a primary cause, and assess whether the AV materially contributed to the event. Our findings show that (1) CRASH attributes 64% of incidents to perception or planning failures, underscoring the importance of reasoning-based analysis for accurate fault attribution; and (2) approximately 50% of reported incidents involve rear-end collisions, highlighting a persistent and unresolved challenge in autonomous driving deployment. We further validate CRASH with five domain experts, achieving 86% accuracy in attributing AV system failures. Overall, CRASH demonstrates strong potential as a scalable and interpretable tool for automated crash analysis, providing actionable insights to support safety research and the continued development of autonomous driving systems.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.15364v1)
