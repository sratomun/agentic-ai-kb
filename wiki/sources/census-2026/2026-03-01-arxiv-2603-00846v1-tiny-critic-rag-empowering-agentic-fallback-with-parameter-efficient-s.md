---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Tiny-Critic RAG: Empowering Agentic Fallback with Parameter-Efficient Small Language Models"
authors: Yichao Wu et al.
url: https://arxiv.org/abs/2603.00846v1
date: 2026-03-01
score: 17
primary: cs.IR
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, post-training, reasoning-models]
---

# Tiny-Critic RAG: Empowering Agentic Fallback with Parameter-Efficient Small Language Models

**arXiv:** [2603.00846v1](https://arxiv.org/abs/2603.00846v1) · 2026-03-01 · cs.IR
**Authors:** Yichao Wu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) grounds Large Language Models (LLMs) to mitigate factual hallucinations. Recent paradigms shift from static pipelines to Modular and Agentic RAG frameworks, granting models autonomy for multi-hop reasoning or self-correction. However, current reflective RAG heavily relies on massive LLMs as universal evaluators. In high-throughput systems, executing complete forward passes for billion-parameter models merely for binary routing introduces severe computational redundancy. Furthermore, in autonomous agent scenarios, inaccurate retrieval causes models to expend excessive tokens on spurious reasoning and redundant tool calls, inflating Time-to-First-Token (TTFT) and costs. We propose Tiny-Critic RAG, decoupling evaluation by deploying a parameter-efficient Small Language Model (SLM) via Low-Rank Adaptation (LoRA). Acting as a deterministic gatekeeper, Tiny-Critic employs constrained decoding and non-thinking inference modes for ultra-low latency binary routing. Evaluations on noise-injected datasets demonstrate Tiny-Critic RAG achieves routing accuracy comparable to GPT-4o-mini while reducing latency by an order of magnitude, establishing a highly cost-effective paradigm for agent deployment.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00846v1)
