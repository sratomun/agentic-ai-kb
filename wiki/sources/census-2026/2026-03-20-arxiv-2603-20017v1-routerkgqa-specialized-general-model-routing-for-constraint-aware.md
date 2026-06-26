---
type: source
source_type: arxiv
title: "RouterKGQA: Specialized--General Model Routing for Constraint-Aware Knowledge Graph Question Answering"
authors: Bo Yuan, Hexuan Deng, Xuebo Liu, Min Zhang
url: https://arxiv.org/abs/2603.20017v1
date: 2026-03-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.CL
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# RouterKGQA: Specialized--General Model Routing for Constraint-Aware Knowledge Graph Question Answering

**arXiv:** [2603.20017v1](https://arxiv.org/abs/2603.20017v1) · 2026-03-20 · cs.CL
**Authors:** Bo Yuan, Hexuan Deng, Xuebo Liu, Min Zhang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Knowledge graph question answering (KGQA) is a promising approach for mitigating LLM hallucination by grounding reasoning in structured and verifiable knowledge graphs. Existing approaches fall into two paradigms: retrieval-based methods utilize small specialized models, which are efficient but often produce unreachable paths and miss implicit constraints, while agent-based methods utilize large general models, which achieve stronger structural grounding at substantially higher cost. We propose RouterKGQA, a framework for specialized--general model collaboration, in which a specialized model generates reasoning paths and a general model performs KG-guided repair only when needed, improving performance at minimal cost. We further equip the specialized with constraint-aware answer filtering, which reduces redundant answers. In addition, we design a more efficient general agent workflow, further lowering inference cost. Experimental results show that RouterKGQA outperforms the previous best by 3.57 points in F1 and 0.49 points in Hits@1 on average across benchmarks, while requiring only 1.15 average LLM calls per question. Codes and models are available at https://github.com/Oldcircle/RouterKGQA.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.20017v1)
