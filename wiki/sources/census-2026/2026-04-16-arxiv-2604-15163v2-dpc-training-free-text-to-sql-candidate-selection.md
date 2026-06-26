---
type: source
source_type: arxiv
title: "DPC: Training-Free Text-to-SQL Candidate Selection via Dual-Paradigm Consistency"
authors: Boyan Li, Ou Ocean Kun Hei, Yue Yu, Yuyu Luo
url: https://arxiv.org/abs/2604.15163v2
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.DB
tags: [data-query-agents, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# DPC: Training-Free Text-to-SQL Candidate Selection via Dual-Paradigm Consistency

**arXiv:** [2604.15163v2](https://arxiv.org/abs/2604.15163v2) · 2026-04-16 · cs.DB
**Authors:** Boyan Li, Ou Ocean Kun Hei, Yue Yu, Yuyu Luo

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Large Language Models (LLMs) demonstrate impressive proficiency in generating SQL queries, they fundamentally lack the capability to self-evaluate correctness without an execution oracle. This limitation creates a stark Generation-Selection Gap, where high potential accuracy (Pass@K) fails to translate into execution accuracy (Pass@1). Although supervised verifiers offer mitigation, they incur prohibitive annotation costs and suffer from domain fragility. Consequently, recent research has pivoted to the training-free setting. However, existing methods--such as Self-Consistency or LLM-as-a-Judge--remain hampered by systematic bias (consensus on hallucinations) and symbolic blindness (inability to simulate execution states). We introduce DPC (Dual-Paradigm Consistency), a multi-agent framework that reformulates SQL selection from a probabilistic guessing task on hidden data into a deterministic verification task on visible data. Specifically, DPC employs a SLICER and a TESTER agent to collaboratively construct a Minimal Distinguishing Database (MDD)--an adversarial, fully observable micro-environment engineered to expose logical discrepancies between candidates. To break the self-correction bias, a SOLVER agent then verifies the SQL candidates by cross-referencing their execution against a parallel Python/Pandas solution. By validating execution consistency between declarative (SQL) and imperative (Python) paradigms, DPC robustly discriminates correct logic from systematic hallucinations. Experiments on BIRD and Spider across multiple LLMs demonstrate that our method consistently outperforms existing selection baselines, achieving absolute accuracy improvements of up to 2.2% over strong competitors like Self-Consistency.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[bird-benchmark]] · [[spider-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.15163v2)
