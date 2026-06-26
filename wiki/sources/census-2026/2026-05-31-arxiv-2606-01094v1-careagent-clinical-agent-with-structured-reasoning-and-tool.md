---
type: source
source_type: arxiv
title: "CAREAgent: Clinical Agent with Structured Reasoning and Tool-Integrated for Order Generation"
authors: Ruihui Hou, Ziyue Huai, Chennuo Zhang, Ziyan Liu et al.
url: https://arxiv.org/abs/2606.01094v1
date: 2026-05-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [clinical-agents, agentic-rl, multi-agent-systems, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# CAREAgent: Clinical Agent with Structured Reasoning and Tool-Integrated for Order Generation

**arXiv:** [2606.01094v1](https://arxiv.org/abs/2606.01094v1) · 2026-05-31 · cs.AI
**Authors:** Ruihui Hou, Ziyue Huai, Chennuo Zhang, Ziyan Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Clinical order generation serves as a critical bridge between clinical decision-making and real-world practice, translating medical decisions into concrete and executable orders. Existing agents mainly focus on coarse-grained decisions and overlook the fine-grained, executable information required for clinical orders. To address this gap, we propose CAREAgent, an agent for clinical order generation. To support its training, we introduce a two-stage agentic reasoning data construction method. First, we design an agent framework that constructs verifiable reasoning trajectories aligned with realistic clinical tool usage. Second, we filter reasoning trajectories by format compliance, order validity, and clinical plausibility. Building on the constructed data, the model is first trained via supervised fine-tuning to acquire fundamental reasoning formats and medical knowledge, and is subsequently optimized through reinforcement learning with multi-dimensional reward functions to enhance complex clinical reasoning capabilities. Experiments on multiple benchmarks demonstrate the effectiveness of CAREAgent. On ClinicalBench (unseen during training), CAREAgent improves the F1 score by 5.05%, 2.09%, and 0.86% over the single-agent, multi-agent, and agentic reasoning methods, respectively.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.01094v1)
