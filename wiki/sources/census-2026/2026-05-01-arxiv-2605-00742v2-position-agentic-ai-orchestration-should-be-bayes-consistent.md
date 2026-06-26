---
type: source
source_type: arxiv
title: "Position: agentic AI orchestration should be Bayes-consistent"
authors: Theodore Papamarkou, Pierre Alquier, Matthias Bauer, Wray Buntine et al.
url: https://arxiv.org/abs/2605.00742v2
date: 2026-05-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [human-agent-interaction, multi-agent-systems, arxiv, auto-ingested]
---

# Position: agentic AI orchestration should be Bayes-consistent

**arXiv:** [2605.00742v2](https://arxiv.org/abs/2605.00742v2) · 2026-05-01 · cs.AI
**Authors:** Theodore Papamarkou, Pierre Alquier, Matthias Bauer, Wray Buntine et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLMs excel at predictive tasks and complex reasoning tasks, but many high-value deployments rely on decisions under uncertainty, for example, which tool to call, which expert to consult, or how many resources to invest. While the usefulness and feasibility of Bayesian approaches remain unclear for LLM inference, this position paper argues that the control layer of an agentic AI system (that orchestrates LLMs and tools) is a clear case where Bayesian principles should shine. Bayesian decision theory provides a framework for agentic systems that can help to maintain beliefs over task-relevant latent quantities, to update these beliefs from observed agentic and human-AI interactions, and to choose actions. Making LLMs themselves explicitly Bayesian belief-updating engines remains computationally intensive and conceptually nontrivial as a general modeling target. In contrast, this paper argues that coherent decision-making requires Bayesian principles at the orchestration level of the agentic system, not necessarily the LLM agent parameters. This paper articulates practical properties for Bayesian control that fit modern agentic AI systems and human-AI collaboration, and provides concrete examples and design patterns to illustrate how calibrated beliefs and utility-aware policies can improve agentic AI orchestration.

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.00742v2)
