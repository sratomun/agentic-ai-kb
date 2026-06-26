---
type: source
source_type: arxiv
title: "Mitigating Cultural Bias in LLMs via Multi-Agent Cultural Debate"
authors: Qian Tan, Lei Jiang, Yuting Zeng, Shuoyang Ding et al.
url: https://arxiv.org/abs/2601.12091v1
date: 2026-01-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.LG
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Mitigating Cultural Bias in LLMs via Multi-Agent Cultural Debate

**arXiv:** [2601.12091v1](https://arxiv.org/abs/2601.12091v1) · 2026-01-17 · cs.LG
**Authors:** Qian Tan, Lei Jiang, Yuting Zeng, Shuoyang Ding et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) exhibit systematic Western-centric bias, yet whether prompting in non-Western languages (e.g., Chinese) can mitigate this remains understudied. Answering this question requires rigorous evaluation and effective mitigation, but existing approaches fall short on both fronts: evaluation methods force outputs into predefined cultural categories without a neutral option, while mitigation relies on expensive multi-cultural corpora or agent frameworks that use functional roles (e.g., Planner--Critique) lacking explicit cultural representation. To address these gaps, we introduce CEBiasBench, a Chinese--English bilingual benchmark, and Multi-Agent Vote (MAV), which enables explicit ``no bias'' judgments. Using this framework, we find that Chinese prompting merely shifts bias toward East Asian perspectives rather than eliminating it. To mitigate such persistent bias, we propose Multi-Agent Cultural Debate (MACD), a training-free framework that assigns agents distinct cultural personas and orchestrates deliberation via a "Seeking Common Ground while Reserving Differences" strategy. Experiments demonstrate that MACD achieves 57.6% average No Bias Rate evaluated by LLM-as-judge and 86.0% evaluated by MAV (vs. 47.6% and 69.0% baseline using GPT-4o as backbone) on CEBiasBench and generalizes to the Arabic CAMeL benchmark, confirming that explicit cultural representation in agent frameworks is essential for cross-cultural fairness.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.12091v1)
