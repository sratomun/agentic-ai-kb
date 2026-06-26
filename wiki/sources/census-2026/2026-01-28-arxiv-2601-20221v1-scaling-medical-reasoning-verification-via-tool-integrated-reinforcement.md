---
type: source
source_type: arxiv
title: "Scaling Medical Reasoning Verification via Tool-Integrated Reinforcement Learning"
authors: Hang Zhang, Ruheng Wang, Yuelyu Ji, Mingu Kwak et al.
url: https://arxiv.org/abs/2601.20221v1
date: 2026-01-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, agent-reliability, agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Scaling Medical Reasoning Verification via Tool-Integrated Reinforcement Learning

**arXiv:** [2601.20221v1](https://arxiv.org/abs/2601.20221v1) · 2026-01-28 · cs.AI
**Authors:** Hang Zhang, Ruheng Wang, Yuelyu Ji, Mingu Kwak et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models have achieved strong performance on medical reasoning benchmarks, yet their deployment in clinical settings demands rigorous verification to ensure factual accuracy. While reward models offer a scalable approach for reasoning trace verification, existing methods face two limitations: they produce only scalar reward values without explicit justification, and they rely on single-pass retrieval that precludes adaptive knowledge access as verification unfolds. We introduce $\method$, an agentic framework that addresses these limitations by training medical reasoning verifiers to iteratively query external medical corpora during evaluation. Our approach combines tool-augmented verification with an iterative reinforcement learning paradigm that requires only trace-level supervision, alongside an adaptive curriculum mechanism that dynamically adjusts training data distribution. Across four medical reasoning benchmarks, $\method$ achieves substantial gains over existing methods, improving MedQA accuracy by 23.5% and MedXpertQA by 32.0% relative to the base generator in particular. Crucially, $\method$ demonstrates an $\mathbf{8\times}$ reduction in sampling budget requirement compared to prior reward model baselines. These findings establish that grounding verification in dynamically retrieved evidence offers a principled path toward more reliable medical reasoning systems.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.20221v1)
