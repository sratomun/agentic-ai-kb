---
type: source
source_type: arxiv
title: "MAVEN: Improving Generalization in Agentic Tool Calling"
authors: Omkar Ghugarkar, Vishvesh Bhat, Muhammad Ahmed Mohsin, Asad Aali
url: https://arxiv.org/abs/2605.30738v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agent-reliability, agent-security, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MAVEN: Improving Generalization in Agentic Tool Calling

**arXiv:** [2605.30738v1](https://arxiv.org/abs/2605.30738v1) · 2026-05-29 · cs.AI
**Authors:** Omkar Ghugarkar, Vishvesh Bhat, Muhammad Ahmed Mohsin, Asad Aali

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Generalization across agentic tool-calling environments remains a central challenge for reliable agentic reasoning systems. Although large language models achieve strong results on individual benchmarks, their ability to compose reasoning strategies, preserve intermediate states, and coordinate tools across domains remains underexplored. We present MAVEN (Modular Agentic Verification and Execution Network), a lightweight symbolic reasoning scaffold for structured decomposition, adaptive tool orchestration, and intermediate verification. We evaluate MAVEN across established tool-calling benchmarks, including BFCL v3, TauBench, Tau2Bench, AceBench, and introduce MAVEN-Bench, a stress-test benchmark for multi-step mathematical and physical reasoning with explicit verification and adversarial task composition. MAVEN-Bench exposes a substantial gap between partial reasoning quality and end-to-end task success; in direct MAVEN-Bench runs, MAVEN improves its GPT-OSS-120b base model from 48% to 71% accuracy without additional training. It also remains competitive with frontier proprietary baselines while using an open-weight backbone with an estimated cost ratio of roughly 1/10, suggesting that lightweight verification-centered scaffolds can strengthen compositional reasoning and motivate more process-aware evaluation of agents in the wild.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bfcl]] · [[tau-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.30738v1)
