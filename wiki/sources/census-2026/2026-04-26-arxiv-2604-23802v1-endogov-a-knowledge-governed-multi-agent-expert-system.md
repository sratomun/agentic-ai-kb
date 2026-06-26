---
type: source
source_type: arxiv
title: "EndoGov: A knowledge-governed multi-agent expert system for endometrial cancer risk stratification"
authors: Weiye Dai, Liyun Shi, Zanxiang He, Yuling Ma et al.
url: https://arxiv.org/abs/2604.23802v1
date: 2026-04-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.MA
tags: [clinical-agents, knowledge-graph, agent-security, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# EndoGov: A knowledge-governed multi-agent expert system for endometrial cancer risk stratification

**arXiv:** [2604.23802v1](https://arxiv.org/abs/2604.23802v1) · 2026-04-26 · cs.MA
**Authors:** Weiye Dai, Liyun Shi, Zanxiang He, Yuling Ma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multimodal artificial intelligence models for endometrial cancer (EC) risk stratification typically optimize aggregate predictive performance but provide limited mechanisms for enforcing mandatory guideline overrides, such as assigning POLE-mutated tumors to the low-risk group despite high-grade morphology. We present EndoGov, a two-tier multi-agent expert system that factorizes the decision process as D(x) = G(P(x), R), where specialist agents P extract structured evidence and a governance agent G applies an executable rule set R. Tier 1 comprises pathology, molecular, and clinical agents that independently generate schema-constrained reports from frozen foundation-model features or structured records. Tier 2 queries an evidence-level-weighted Guideline Knowledge Graph, using deterministic hard-path rules for high-priority overrides and constrained soft-path reasoning for ambiguous cases. In TCGA-UCEC (n=541), EndoGov achieved 0.943 accuracy, 0.973 macro AUC, and a conditional logic-violation rate (C-LVR) of 0.93% among trigger-exposed cases. In CPTAC-UCEC (n=95), where reference labels are guideline-derived, EndoGov reached 0.842 accuracy compared with < 0.31 for locked-transfer neural baselines, supporting governance-pathway transfer under distribution shift rather than validation against independent clinical truth. End-to-end safety decomposition localized residual failures primarily to upstream molecular detection rather than downstream governance. Backend-swap experiments further showed that hard-path compliance is invariant to the LLM backend. These findings indicate that explicit clinical-rule governance can provide guideline-compliant, auditable EC risk assignment while preserving competitive discrimination.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.23802v1)
