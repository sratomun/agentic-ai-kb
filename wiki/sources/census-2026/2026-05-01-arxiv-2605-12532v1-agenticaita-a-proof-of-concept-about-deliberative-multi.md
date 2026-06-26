---
type: source
source_type: arxiv
title: "AgenticAITA: A Proof-Of-Concept About Deliberative Multi-Agent Reasoning for Autonomous Trading Systems"
authors: Ivan Letteri
url: https://arxiv.org/abs/2605.12532v1
date: 2026-05-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: q-fin.TR
tags: [finance-agents, agent-economies, agent-security, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# AgenticAITA: A Proof-Of-Concept About Deliberative Multi-Agent Reasoning for Autonomous Trading Systems

**arXiv:** [2605.12532v1](https://arxiv.org/abs/2605.12532v1) · 2026-05-01 · q-fin.TR
**Authors:** Ivan Letteri

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Conventional algorithmic trading systems are grounded in deterministic heuristics or offline-trained statistical models that cannot adapt to the semantic complexity of rapidly shifting market regimes. This paper introduces AGENTICAITA, an agentic AI framework that replaces the traditional signal then execute paradigm with a fully autonomous deliberative loop in which multiple specialized Large Language Model agents reason, negotiate, and act in concert - without any offline training or human intervention. The framework proposes four architectural contributions: (i) an Adaptive Z-Score Trigger Engine that acts as a cognitive resource allocator, gating LLM inference exclusively on statistically anomalous market conditions; (ii) a Sequential Deliberative Pipeline - the core agentic contribution - in which an Analyst agent, a Risk Manager agent, and an Executor agent form a structured reasoning chain governed by typed JSON contracts and a deterministic hard-gate safety layer; (iii) an Inference Gating Protocol, a mutex-based cognitive resource scheduler that serializes concurrent agent activations and ensures fully reproducible audit trails; and (iv) a Correlation-Break Diversification composite score that operationalizes portfolio-level idiosyncratic signal prioritization within individual agent reasoning. Validated over a five-day autonomous dry-run session under live market conditions, the framework demonstrates operational correctness of the deliberative pipeline, achieving 157 zero-intervention invocations across 76 assets with an 11.5% agentic friction rate that confirms non-trivial inter-agent negotiation. This preliminary proof-of-concept establishes the feasibility of training-free, deterministic safety-constrained multi-agent orchestration in financial decision loops, with statistically robust performance evaluation and execution cost modeling deferred to extended live deployment.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-economies|Agent economies]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12532v1)
