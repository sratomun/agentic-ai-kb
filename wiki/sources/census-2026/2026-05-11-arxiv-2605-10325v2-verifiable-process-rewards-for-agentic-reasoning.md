---
type: source
source_type: arxiv
title: "Verifiable Process Rewards for Agentic Reasoning"
authors: Huining Yuan, Zelai Xu, Huaijie Wang, Xiangmin Yi et al.
url: https://arxiv.org/abs/2605.10325v2
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-skills, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Verifiable Process Rewards for Agentic Reasoning

**arXiv:** [2605.10325v2](https://arxiv.org/abs/2605.10325v2) · 2026-05-11 · cs.AI
**Authors:** Huining Yuan, Zelai Xu, Huaijie Wang, Xiangmin Yi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement learning from verifiable rewards (RLVR) has improved the reasoning abilities of large language models (LLMs), but most existing approaches rely on sparse outcome-level feedback. This sparsity creates a credit assignment challenge in long-horizon agentic reasoning: a trajectory may fail despite containing many correct intermediate decisions, or succeed despite containing flawed ones. In this work, we study a class of densely-verifiable agentic reasoning problems, where intermediate actions can be objectively checked by symbolic or algorithmic oracles. We propose Verifiable Process Rewards (VPR), a framework that converts such oracles into dense turn-level supervision for reinforcement learning, and instantiate it in three representative settings: search-based verification for dynamic deduction, constraint-based verification for logical reasoning, and posterior-based verification for probabilistic inference. We further provide a theoretical analysis showing that dense verifier-grounded rewards can improve long-horizon credit assignment by providing more localized learning signals, with the benefit depending on the reliability of the verifier. Empirically, VPR outperforms outcome-level reward and rollout-based process reward baselines across controlled environments, and more importantly, transfers to both general and agentic reasoning benchmarks, suggesting that verifiable process supervision can foster general reasoning skills applicable beyond the training environments. Our results indicate that VPR is a promising approach for enhancing LLM agents whenever reliable intermediate verification is available, while also highlighting its dependence on oracle quality and the open challenge of extending VPR to less structured, open-ended environments.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-skills|Agent skills]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.10325v2)
