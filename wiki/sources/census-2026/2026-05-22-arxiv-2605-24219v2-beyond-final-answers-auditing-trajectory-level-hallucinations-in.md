---
type: source
source_type: arxiv
title: "Beyond Final Answers: Auditing Trajectory-Level Hallucinations in Multi-Agent Industrial Workflows"
authors: Harshada Badave, Santosh Borse, Andrea Gomez, Harshitha Narahari et al.
url: https://arxiv.org/abs/2605.24219v2
date: 2026-05-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [multi-agent-systems, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Beyond Final Answers: Auditing Trajectory-Level Hallucinations in Multi-Agent Industrial Workflows

**arXiv:** [2605.24219v2](https://arxiv.org/abs/2605.24219v2) · 2026-05-22 · cs.AI
**Authors:** Harshada Badave, Santosh Borse, Andrea Gomez, Harshitha Narahari et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) are increasingly deployed as autonomous agents that reason, use tools, and act over multiple steps. Yet most hallucination benchmarks still evaluate only the final output, missing failures that originate in intermediate Thought-Action-Observation steps. We present Trajel, a dataset and evaluation framework for auditing trajectory-level hallucinations in multi-agent industrial workflows. Trajel introduces a five-type hallucination taxonomy (factual, referential, logical, procedural, and scope-based) over expert-annotated agent traces from AssetOpsBench. We benchmark supervised detection models at the subtask, trajectory, and long-context levels. Our results show that the most common failure modes are missed by existing benchmarks, that nearly half of hallucinated trajectories involve multiple types at once, and that automated detectors with high binary accuracy still misclassify the subtlest types. Trajectory-aware detection significantly outperforms standard post-hoc verification, making taxonomy-grounded evaluation necessary for safer agentic deployment.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.24219v2)
