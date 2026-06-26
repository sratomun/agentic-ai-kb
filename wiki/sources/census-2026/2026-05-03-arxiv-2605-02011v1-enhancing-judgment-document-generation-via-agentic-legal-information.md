---
type: source
source_type: arxiv
title: "Enhancing Judgment Document Generation via Agentic Legal Information Collection and Rubric-Guided Optimization"
authors: Weihang Su, Xuanyi Chen, Yueyue Wu, Qingyao Ai et al.
url: https://arxiv.org/abs/2605.02011v1
date: 2026-05-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [agentic-rl, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Enhancing Judgment Document Generation via Agentic Legal Information Collection and Rubric-Guided Optimization

**arXiv:** [2605.02011v1](https://arxiv.org/abs/2605.02011v1) · 2026-05-03 · cs.CL
**Authors:** Weihang Su, Xuanyi Chen, Yueyue Wu, Qingyao Ai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Automating the drafting of judgment documents is pivotal to judicial efficiency, yet it remains challenging due to the dual requirements of comprehensive retrieval of legal information and rigorous logical reasoning. Existing approaches, typically relying on standard Retrieval-Augmented Generation and Supervised Fine-Tuning, often suffer from insufficient evidence recall, hallucinated statutory references, and logically flawed legal reasoning. To bridge this gap, we propose Judge-R1, a unified framework designed to enhance LLM-based judgment document generation by jointly improving legal information collection and judgment document generation. First, we introduce Agentic Legal Information Collection, which employs a dynamic planning agent to retrieve precise statutes and precedents from multiple sources. Second, we implement Rubric-Guided Optimization, a reinforcement learning phase utilizing Group Relative Policy Optimization (GRPO) with a comprehensive legal reward function to enforce adherence to judicial standards and reasoning logic. Extensive experiments on the JuDGE benchmark demonstrate that Judge-R1 significantly outperforms state-of-the-art baselines in both legal accuracy and generation quality.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02011v1)
