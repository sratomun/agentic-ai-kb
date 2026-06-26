---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "SLMJury: Can Small Language Models Judge as Well as Large Ones?"
authors: Anish Laddha et al.
url: https://arxiv.org/abs/2606.07810v1
date: 2026-06-05
score: 6
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, reasoning-models, multi-agent-systems]
---

# SLMJury: Can Small Language Models Judge as Well as Large Ones?

**arXiv:** [2606.07810v1](https://arxiv.org/abs/2606.07810v1) · 2026-06-05 · cs.CL
**Authors:** Anish Laddha et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) are widely used as judges for evaluating model outputs, but their high cost, latency, and opacity limit scalability. We introduce SLMJury, a framework for evaluating small language models (SLMs) as judges across two paradigms: closed-ended binary correctness and open-ended quality scoring. We benchmark 16 SLM judges (0.6B-14B parameters) from four model families across ten benchmarks: eight closed-ended tasks spanning mathematical, scientific, and general reasoning (N=64,824 judgments per configuration), plus SummEval and MT-Bench for summarization and conversational scoring. We formalize judging as a budget-conditioned function and study five dimensions. Four findings emerge. (1) The overthinking effect is domain-dependent: for most judges quick 10-token verdicts match or beat extended reasoning on mathematical judging (by 2-7% where they help), while reasoning wins on general tasks by up to 23%. (2) Domain generalization separates model families, with math-to-general accuracy gaps ranging from under 10% to nearly 40%. (3) Closed-ended and open-ended judging draw on different capabilities: the best binary judge (Phi-4) drops to rank 9 on MT-Bench, while reasoning-trained models invert this ordering. (4) Under the Reflect-Critique-Refine (RCR) debate protocol, multi-agent debate degrades accuracy across all tested configurations, whereas the top judges resist six adversarial personas with <=0.55% variance. Reliable automated evaluation does not require large proprietary models, yet no single SLM dominates. The leaderboard is available at https://anishh15.github.io/SLMJury/, and our framework code and pip package are publicly available at https://github.com/anishh15/SLMJury and https://pypi.org/project/slmjury/.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[reasoning-models]] · [[multi-agent-systems]]
- **Entities:** [[phi]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.07810v1)
