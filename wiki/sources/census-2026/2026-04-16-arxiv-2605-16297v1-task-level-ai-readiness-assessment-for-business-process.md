---
type: source
source_type: arxiv
title: "Task-Level AI Readiness Assessment for Business Process Management:The T-IPO Model and LARA Matrix in Financial-Services IT Operations"
authors: Mingjun Li, Xiaojun Ye
url: https://arxiv.org/abs/2605.16297v1
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.CY
tags: [finance-agents, knowledge-graph, agent-reliability, governance-gap, arxiv, auto-ingested]
---

# Task-Level AI Readiness Assessment for Business Process Management:The T-IPO Model and LARA Matrix in Financial-Services IT Operations

**arXiv:** [2605.16297v1](https://arxiv.org/abs/2605.16297v1) · 2026-04-16 · cs.CY
**Authors:** Mingjun Li, Xiaojun Ye

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Which tasks inside an enterprise workflow can a large-language-model agent reliably handle, and under what conditions? Most business process modeling frameworks still answer this at the activity level, even though a single activity can bundle work of radically different difficulty. This paper takes the analysis a step smaller. We describe two design artifacts developed in a financial-services IT setting: T-IPO, which represents each task as an eight-element tuple, and LARA (LLM Agent Readiness Assessment), a five-dimension rubric that scores a task's readiness for agent substitution. Compliance Sensitivity carries $1.5\times$ weight, a value we fixed through a three-round Delphi study and cross-checked with AHP. The rubric produces four levels, L1 to L4, and applies a floor rule so that a task with maximum compliance load cannot be classified below L3 no matter what the other scores say. Both artifacts sit inside a larger methodology (PARTIS) that we map onto BWW ontology in Section 3. We evaluate the instruments across 127 tasks. Inter-rater agreement reaches Fleiss' $κ= 0.80$; a replication at three further institutions returns $κ= 0.73$. A controlled comparison against activity-level assessment suggests, though does not prove, an improvement in predictive utility at the task level. Pilot deployment of 120 task instances confirms that auto-completion decays monotonically from $95\%$ at L1 through about $70\%$ at L2 to about $40\%$ at L3. Exploratory factor analysis points to a two-factor structure: task readiness seems to be determined jointly by cognitive-execution complexity and governance-compliance intensity. We close with a recalibration procedure (LARA-TCA) so the rubric can keep pace with evolving LLM capabilities.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16297v1)
