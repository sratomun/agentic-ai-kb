---
type: source
source_type: arxiv
title: "BIRDTurk: Adaptation of the BIRD Text-to-SQL Dataset to Turkish"
authors: Burak Aktaş, Mehmet Can Baytekin, Süha Kağan Köse, Ömer İlbilgi et al.
url: https://arxiv.org/abs/2602.03633v1
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.CL
tags: [data-query-agents, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# BIRDTurk: Adaptation of the BIRD Text-to-SQL Dataset to Turkish

**arXiv:** [2602.03633v1](https://arxiv.org/abs/2602.03633v1) · 2026-02-03 · cs.CL
**Authors:** Burak Aktaş, Mehmet Can Baytekin, Süha Kağan Köse, Ömer İlbilgi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text-to-SQL systems have achieved strong performance on English benchmarks, yet their behavior in morphologically rich, low-resource languages remains largely unexplored. We introduce BIRDTurk, the first Turkish adaptation of the BIRD benchmark, constructed through a controlled translation pipeline that adapts schema identifiers to Turkish while strictly preserving the logical structure and execution semantics of SQL queries and databases. Translation quality is validated on a sample size determined by the Central Limit Theorem to ensure 95% confidence, achieving 98.15% accuracy on human-evaluated samples. Using BIRDTurk, we evaluate inference-based prompting, agentic multi-stage reasoning, and supervised fine-tuning. Our results reveal that Turkish introduces consistent performance degradation, driven by both structural linguistic divergence and underrepresentation in LLM pretraining, while agentic reasoning demonstrates stronger cross-lingual robustness. Supervised fine-tuning remains challenging for standard multilingual baselines but scales effectively with modern instruction-tuned models. BIRDTurk provides a controlled testbed for cross-lingual Text-to-SQL evaluation under realistic database conditions. We release the training and development splits to support future research.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.03633v1)
