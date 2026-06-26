---
type: source
source_type: arxiv
title: "Uncertainty-Aware Clarification in LLM Agents with Information Gain"
authors: Mengyi Deng, Zhiwei Li, Xin Li et al.
url: https://arxiv.org/abs/2606.03135v1
date: 2026-06-02
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [intent-understanding, human-agent-interaction, arxiv, auto-ingested]
---

# Uncertainty-Aware Clarification in LLM Agents with Information Gain

**arXiv:** [2606.03135v1](https://arxiv.org/abs/2606.03135v1) · 2026-06-02 · cs.AI
**Authors:** Mengyi Deng, Zhiwei Li, Xin Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
Large Language Model (LLM) agents often operate under underspecified user instructions, where latent uncertainty over user intent leads to erroneous tool actions. To address this challenge, we propose a goal-oriented clarification framework that aligns clarification behavior with ambiguity resolution. Central to our approach is the Information Gain Reward, a metric that quantifies the utility of clarification questions by measuring the Bayesian belief update towards the ground-truth goal induced by the clarification exchange. We train the clarifier (LLM) using this reward to optimize for high information gain, ensuring that clarifications effectively reduce uncertainty and improve task completion within the agent-tool-user environment. We validate our framework within a clarification-enhanced $τ$-Bench environment, conducting cross-agent evaluations across five heterogeneous backbones. Empirical results demonstrate that our method consistently improves the success rate by 3.7\% over the no-clarification baseline, while adding only 0.3 total interaction steps on average.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[human-agent-interaction|Human-agent interaction]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03135v1)
