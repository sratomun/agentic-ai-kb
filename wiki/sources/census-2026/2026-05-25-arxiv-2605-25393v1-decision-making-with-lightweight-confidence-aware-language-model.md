---
type: source
source_type: arxiv
title: "Decision-Making with Lightweight Confidence-Aware Language Model for Autonomous Driving"
authors: Ruoyu Yao, Ruiguo Zhong, Pei Liu, Mingxing Peng et al.
url: https://arxiv.org/abs/2605.25393v1
date: 2026-05-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.RO
tags: [autonomous-driving-agents, agentic-rag, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Decision-Making with Lightweight Confidence-Aware Language Model for Autonomous Driving

**arXiv:** [2605.25393v1](https://arxiv.org/abs/2605.25393v1) · 2026-05-25 · cs.RO
**Authors:** Ruoyu Yao, Ruiguo Zhong, Pei Liu, Mingxing Peng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) and Multimodal LLMs (MLLMs) have demonstrated immense potential in autonomous driving (AD) by offering human-like reasoning and open-world generalization. However, the excessive computational overhead and high inference latency of these massive models severely hinder their deployment in resource-constrained AD systems. To address this challenge, we propose a novel decision-making framework utilizing a lightweight confidence-aware language model, which bridges the gap between complex multimodal intention reasoning and efficient inference. Specifically, we design a multi-agent collaborative workflow, comprising action voting, confidence assessment, and summarization agents, to generate high-quality, confidence-annotated decision demonstrations via explicit Chain-of-Thought (CoT) reasoning. These demonstrations are then distilled into a lightweight language model featuring a dual-head architecture, enabling the joint prediction of decision probabilities and the generation of textual rationales. The distillation is realized via a confidence-aware fine-tuning strategy coupled with Retrieval Augmented Generation (RAG) to enhance the model's adaptability and data efficiency. Comprehensive closed-loop experiments on the nuPlan benchmark demonstrate that our approach achieves state-of-the-art (SOTA) success rates in both regular and long-tail scenarios while maintaining low inference latency.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.25393v1)
