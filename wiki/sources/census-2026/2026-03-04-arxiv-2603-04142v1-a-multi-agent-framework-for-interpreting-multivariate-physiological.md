---
type: source
source_type: arxiv
title: "A Multi-Agent Framework for Interpreting Multivariate Physiological Time Series"
authors: Davide Gabrielli, Paola Velardi, Stefano Faralli, Bardh Prenkaj
url: https://arxiv.org/abs/2603.04142v1
date: 2026-03-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.LG
tags: [clinical-agents, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# A Multi-Agent Framework for Interpreting Multivariate Physiological Time Series

**arXiv:** [2603.04142v1](https://arxiv.org/abs/2603.04142v1) · 2026-03-04 · cs.LG
**Authors:** Davide Gabrielli, Paola Velardi, Stefano Faralli, Bardh Prenkaj

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Continuous physiological monitoring is central to emergency care, yet deploying trustworthy AI is challenging. While LLMs can translate complex physiological signals into clinical narratives, it is unclear how agentic systems perform relative to zero-shot inference. To address these questions, we present Vivaldi, a role-structured multi-agent system that explains multivariate physiological time series. Due to regulatory constraints that preclude live deployment, we instantiate Vivaldi in a controlled, clinical pilot to a small, highly qualified cohort of emergency medicine experts, whose evaluations reveal a context-dependent picture that contrasts with prevailing assumptions that agentic reasoning uniformly improves performance. Our experiments show that agentic pipelines substantially benefit non-thinking and medically fine-tuned models, improving expert-rated explanation justification and relevance by +6.9 and +9.7 points, respectively. Contrarily, for thinking models, agentic orchestration often degrades explanation quality, including a 14-point drop in relevance, while improving diagnostic precision (ESI F1 +3.6). We also find that explicit tool-based computation is decisive for codifiable clinical metrics, whereas subjective targets, such as pain scores and length of stay, show limited or inconsistent changes. Expert evaluation further indicates that gains in clinical utility depend on visualization conventions, with medically specialized models achieving the most favorable trade-offs between utility and clarity. Together, these findings show that the value of agentic AI lies in the selective externalization of computation and structure rather than in maximal reasoning complexity, and highlight concrete design trade-offs and learned lessons, broadly applicable to explainable AI in safety-critical healthcare settings.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.04142v1)
