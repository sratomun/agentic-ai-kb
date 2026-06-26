---
type: source
source_type: arxiv
title: "MedCollab: IBIS-Guided Multi-Agent Collaboration with Hierarchical Disease Relation Chains for Clinical Diagnosis"
authors: Yuqi Zhan, Xinyue Wu, Tianyu Lin, Yutong Bao et al.
url: https://arxiv.org/abs/2603.01131v3
date: 2026-03-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [clinical-agents, agent-protocols, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# MedCollab: IBIS-Guided Multi-Agent Collaboration with Hierarchical Disease Relation Chains for Clinical Diagnosis

**arXiv:** [2603.01131v3](https://arxiv.org/abs/2603.01131v3) · 2026-03-01 · cs.MA
**Authors:** Yuqi Zhan, Xinyue Wu, Tianyu Lin, Yutong Bao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Clinical diagnosis is a gradual process of evidence integration, in which physicians move from symptoms and medical history to examinations, competing hypotheses, disease relations, and treatment decisions. Large language models have advanced medical text understanding and generation. Yet their clinical use remains limited by weak evidence grounding, opaque reasoning, and inconsistent links among differential diagnosis, final diagnosis, diagnostic basis, and treatment planning. We introduce MedCollab, a multi-agent framework for full-cycle clinical diagnosis and report generation. MedCollab coordinates specialist and examination agents according to patient records. It structures agent deliberation with an Issue-Based Information System (IBIS) protocol, so that each diagnostic position is supported by patient-specific evidence and medical knowledge. It also builds Hierarchical Disease Relation Chains (HDRC) to connect accepted hypotheses through progression, complication, and comorbidity relations. During multi-round deliberation, a verifier-guided consensus module evaluates evidence support, medical plausibility, and logical conflicts. It then adjusts agent contributions and filters unsupported reasoning. Experiments on ClinicalBench and MIMIC-IV show that MedCollab outperforms leading LLMs and medical multi-agent baselines in diagnostic accuracy, evidence consistency, and clinical reasoning quality. These results indicate that structured and auditable collaboration can produce more faithful and clinically coherent diagnostic reports.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01131v3)
