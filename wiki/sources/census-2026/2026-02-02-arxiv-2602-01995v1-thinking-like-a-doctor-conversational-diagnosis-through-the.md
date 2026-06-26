---
type: source
source_type: arxiv
title: "Thinking Like a Doctor: Conversational Diagnosis through the Exploration of Diagnostic Knowledge Graphs"
authors: Jeongmoon Won, Seungwon Kook, Yohan Jo
url: https://arxiv.org/abs/2602.01995v1
date: 2026-02-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.AI
tags: [clinical-agents, knowledge-graph, arxiv, auto-ingested]
---

# Thinking Like a Doctor: Conversational Diagnosis through the Exploration of Diagnostic Knowledge Graphs

**arXiv:** [2602.01995v1](https://arxiv.org/abs/2602.01995v1) · 2026-02-02 · cs.AI
**Authors:** Jeongmoon Won, Seungwon Kook, Yohan Jo

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Conversational diagnosis requires multi-turn history-taking, where an agent asks clarifying questions to refine differential diagnoses under incomplete information. Existing approaches often rely on the parametric knowledge of a model or assume that patients provide rich and concrete information, which is unrealistic. To address these limitations, we propose a conversational diagnosis system that explores a diagnostic knowledge graph to reason in two steps: (i) generating diagnostic hypotheses from the dialogue context, and (ii) verifying hypotheses through clarifying questions, which are repeated until a final diagnosis is reached. Since evaluating the system requires a realistic patient simulator that responds to the system's questions, we adopt a well-established simulator along with patient profiles from MIMIC-IV. We further adapt it to describe symptoms vaguely to reflect real-world patients during early clinical encounters. Experiments show improved diagnostic accuracy and efficiency over strong baselines, and evaluations by physicians support the realism of our simulator and the clinical utility of the generated questions. Our code will be released upon publication.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.01995v1)
