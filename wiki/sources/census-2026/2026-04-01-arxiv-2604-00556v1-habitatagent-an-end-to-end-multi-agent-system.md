---
type: source
source_type: arxiv
title: "HabitatAgent: An End-to-End Multi-Agent System for Housing Consultation"
authors: Hongyang Yang, Yanxin Zhang, Yang She, Yue Xiao et al.
url: https://arxiv.org/abs/2604.00556v1
date: 2026-04-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.LG
tags: [recommendation-agents, knowledge-graph, agent-reliability, agent-protocols, agent-memory, arxiv, auto-ingested]
---

# HabitatAgent: An End-to-End Multi-Agent System for Housing Consultation

**arXiv:** [2604.00556v1](https://arxiv.org/abs/2604.00556v1) · 2026-04-01 · cs.LG
**Authors:** Hongyang Yang, Yanxin Zhang, Yang She, Yue Xiao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Housing selection is a high-stakes and largely irreversible decision problem. We study housing consultation as a decision-support interface for housing selection. Existing housing platforms and many LLM-based assistants often reduce this process to ranking or recommendation, resulting in opaque reasoning, brittle multi-constraint handling, and limited guarantees on factuality. We present HabitatAgent, the first LLM-powered multi-agent architecture for end-to-end housing consultation. HabitatAgent comprises four specialized agent roles: Memory, Retrieval, Generation, and Validation. The Memory Agent maintains multi-layer user memory through internal stages for constraint extraction, memory fusion, and verification-gated updates; the Retrieval Agent performs hybrid vector--graph retrieval (GraphRAG); the Generation Agent produces evidence-referenced recommendations and explanations; and the Validation Agent applies multi-tier verification and targeted remediation. Together, these agents provide an auditable and reliable workflow for end-to-end housing consultation. We evaluate HabitatAgent on 100 real user consultation scenarios (300 multi-turn question--answer pairs) under an end-to-end correctness protocol. A strong single-stage baseline (Dense+Rerank) achieves 75% accuracy, while HabitatAgent reaches 95%.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-memory|Agent memory]]
- **Entities:** [[graphrag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.00556v1)
