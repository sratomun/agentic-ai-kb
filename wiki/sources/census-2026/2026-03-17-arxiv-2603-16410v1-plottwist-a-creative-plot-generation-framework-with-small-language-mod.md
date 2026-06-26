---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "PlotTwist: A Creative Plot Generation Framework with Small Language Models"
authors: Abhinav Thorat et al.
url: https://arxiv.org/abs/2603.16410v1
date: 2026-03-17
score: 5
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, clinical-agents]
---

# PlotTwist: A Creative Plot Generation Framework with Small Language Models

**arXiv:** [2603.16410v1](https://arxiv.org/abs/2603.16410v1) · 2026-03-17 · cs.CL
**Authors:** Abhinav Thorat et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Creative plot generation presents a fundamental challenge for language models: transforming a concise premise into a coherent narrative that sustains global structure, character development, and emotional resonance. Although recent Large Language Models (LLMs) demonstrate strong fluency across general-purpose tasks, they typically require preference alignment to perform well on specialized domains such as creative plot generation. However, conducting such alignment at the scale of frontier LLMs is computationally prohibitive, significantly limiting accessibility and practical deployment. To address this, we present PlotTwist, a structured framework that enables Small Language Models (SLMs) with $\leq$ 5B active parameters to generate high-quality, premise-conditioned plots competitive with frontier systems up to $200\times$ larger. Our approach decomposes generation into three specialized components: (1) an Aspect Rating Reward Model trained via a novel Positive-Negative prompting strategy to deliver structured narratives across five Narrative Quality Dimensions (NQDs); (2) a Mixture-of-Experts (MoE) plot generator aligned via Direct Preference Optimization on high-confidence preference pairs; and (3) an Agentic Evaluation module that emulates human critical judgment for unbiased post-hoc assessment. Extensive experiments demonstrate that PlotTwist consistently outperforms frontier models across multiple NQDs despite substantially tighter capacity constraints. Further validation confirms strong sensitivity to narrative quality, as the framework reliably distinguishes plots derived from critically acclaimed versus widely panned screenplays. Together, these results establish structured, preference-based alignment as a resource-efficient approach to high-quality creative plot generation.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[clinical-agents]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.16410v1)
