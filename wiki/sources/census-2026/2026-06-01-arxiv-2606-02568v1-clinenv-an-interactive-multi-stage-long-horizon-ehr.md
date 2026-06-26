---
type: source
source_type: arxiv
title: "ClinEnv: An Interactive Multi-Stage Long Horizon EHR Environment for Agents"
authors: Yuxing Lu, Yushuhong Lin, Wenqi Shi, J. Ben Tamo et al.
url: https://arxiv.org/abs/2606.02568v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-reliability, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# ClinEnv: An Interactive Multi-Stage Long Horizon EHR Environment for Agents

**arXiv:** [2606.02568v1](https://arxiv.org/abs/2606.02568v1) · 2026-06-01 · cs.AI
**Authors:** Yuxing Lu, Yushuhong Lin, Wenqi Shi, J. Ben Tamo et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Clinical practice is not the selection of an answer from enumerated options: a physician gathers heterogeneous information incrementally and commits to sequential, irreversible decisions under uncertainty. Static benchmarks cannot probe and existing interactive medical benchmarks each compromise on at least one of them. We present ClinEnv, an interactive benchmark that evaluates LLMs as attending physicians over real inpatient admissions under a paradigm we term Longitudinal Inpatient Simulation. Each case is automatically constructed into an ordered sequence of decision stages; at every stage the model must actively query four specialized agents before committing to medications, procedures, and diagnoses. ClinEnv scores both what the model decides, through deterministic ontology-grounded matching, and how it gathers information. Across seven models, the strongest reaches only 0.31 decision F1, and outcome quality is sharply decoupled from process quality. Difficulty concentrates in management decisions and later stages, where models recover discharge diagnoses far more reliably than management actions (0.51 vs. 0.17 F1) and continue to issue redundant queries as cases progress. ClinEnv makes this information-acquisition gap, invisible to outcome-only evaluation, directly measurable.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.02568v1)
