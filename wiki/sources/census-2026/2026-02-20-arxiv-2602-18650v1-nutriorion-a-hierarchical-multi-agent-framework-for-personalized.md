---
type: source
source_type: arxiv
title: "NutriOrion: A Hierarchical Multi-Agent Framework for Personalized Nutrition Intervention Grounded in Clinical Guidelines"
authors: Junwei Wu, Runze Yan, Hanqi Luo, Darren Liu et al.
url: https://arxiv.org/abs/2602.18650v1
date: 2026-02-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.MA
tags: [recommendation-agents, clinical-agents, agent-security, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# NutriOrion: A Hierarchical Multi-Agent Framework for Personalized Nutrition Intervention Grounded in Clinical Guidelines

**arXiv:** [2602.18650v1](https://arxiv.org/abs/2602.18650v1) · 2026-02-20 · cs.MA
**Authors:** Junwei Wu, Runze Yan, Hanqi Luo, Darren Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Personalized nutrition intervention for patients with multimorbidity is critical for improving health outcomes, yet remains challenging because it requires the simultaneous integration of heterogeneous clinical conditions, medications, and dietary guidelines. Single-agent large language models (LLMs) often suffer from context overload and attention dilution when processing such high-dimensional patient profiles. We introduce NutriOrion, a hierarchical multi-agent framework with a parallel-then-sequential reasoning topology. NutriOrion decomposes nutrition planning into specialized domain agents with isolated contexts to mitigate anchoring bias, followed by a conditional refinement stage. The framework includes a multi-objective prioritization algorithm to resolve conflicting dietary requirements and a safety constraint mechanism that injects pharmacological contraindications as hard negative constraints during synthesis, ensuring clinical validity by construction rather than post-hoc filtering. For clinical interoperability, NutriOrion maps synthesized insights into the ADIME standard and FHIR R4 resources. Evaluated on 330 stroke patients with multimorbidity, NutriOrion outperforms multiple baselines, including GPT-4.1 and alternative multi-agent architectures. It achieves a 12.1 percent drug-food interaction violation rate, demonstrates strong personalization with negative correlations (-0.26 to -0.35) between patient biomarkers and recommended risk nutrients, and yields clinically meaningful dietary improvements, including a 167 percent increase in fiber and a 27 percent increase in potassium, alongside reductions in sodium (9 percent) and sugars (12 percent).

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[clinical-agents|Clinical agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.18650v1)
