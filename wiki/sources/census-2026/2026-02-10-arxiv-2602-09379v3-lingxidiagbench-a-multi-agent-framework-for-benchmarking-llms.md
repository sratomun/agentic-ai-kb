---
type: source
source_type: arxiv
title: "LingxiDiagBench: A Multi-Agent Framework for Benchmarking LLMs in Chinese Psychiatric Consultation and Diagnosis"
authors: Shihao Xu, Tiancheng Zhou, Jiatong Ma, Yanli Ding et al.
url: https://arxiv.org/abs/2602.09379v3
date: 2026-02-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [clinical-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# LingxiDiagBench: A Multi-Agent Framework for Benchmarking LLMs in Chinese Psychiatric Consultation and Diagnosis

**arXiv:** [2602.09379v3](https://arxiv.org/abs/2602.09379v3) · 2026-02-10 · cs.MA
**Authors:** Shihao Xu, Tiancheng Zhou, Jiatong Ma, Yanli Ding et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Mental disorders are highly prevalent worldwide, but the shortage of psychiatrists and the inherent subjectivity of interview-based diagnosis create substantial barriers to timely and consistent mental-health assessment. Progress in AI-assisted psychiatric diagnosis is constrained by the absence of benchmarks that simultaneously provide realistic patient simulation, clinician-verified diagnostic labels, and support for dynamic multi-turn consultation. We present LingxiDiagBench, a large-scale multi-agent benchmark that evaluates LLMs on both static diagnostic inference and dynamic multi-turn psychiatric consultation in Chinese. At its core is LingxiDiag-16K, a dataset of 16,000 EMR-aligned synthetic consultation dialogues designed to reproduce real clinical demographic and diagnostic distributions across 12 ICD-10 psychiatric categories. Through extensive experiments across state-of-the-art LLMs, we establish key findings: (1) although LLMs achieve high accuracy on binary depression--anxiety classification (up to 92.3%), performance deteriorates substantially for depression--anxiety comorbidity recognition (43.0%) and 12-way differential diagnosis (28.5%); (2) dynamic consultation often underperforms static evaluation, indicating that ineffective information-gathering strategies significantly impair downstream diagnostic reasoning; (3) consultation quality assessed by LLM-as-a-Judge shows only moderate correlation with diagnostic accuracy, suggesting that well-structured questioning alone does not ensure correct diagnostic decisions. We release LingxiDiag-16K and the full evaluation framework to support reproducible research at https://github.com/Lingxi-mental-health/LingxiDiagBench.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.09379v3)
