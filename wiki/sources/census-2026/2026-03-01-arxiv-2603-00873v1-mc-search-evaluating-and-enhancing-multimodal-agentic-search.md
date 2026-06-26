---
type: source
source_type: arxiv
title: "MC-Search: Evaluating and Enhancing Multimodal Agentic Search with Structured Long Reasoning Chains"
authors: Xuying Ning, Dongqi Fu, Tianxin Wei, Mengting Ai et al.
url: https://arxiv.org/abs/2603.00873v1
date: 2026-03-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# MC-Search: Evaluating and Enhancing Multimodal Agentic Search with Structured Long Reasoning Chains

**arXiv:** [2603.00873v1](https://arxiv.org/abs/2603.00873v1) · 2026-03-01 · cs.AI
**Authors:** Xuying Ning, Dongqi Fu, Tianxin Wei, Mengting Ai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
With the increasing demand for step-wise, cross-modal, and knowledge-grounded reasoning, multimodal large language models (MLLMs) are evolving beyond the traditional fixed retrieve-then-generate paradigm toward more sophisticated agentic multimodal retrieval-augmented generation (MM-RAG). Existing benchmarks, however, mainly focus on simplified QA with short retrieval chains, leaving adaptive planning and multimodal reasoning underexplored. We present MC-Search, the first benchmark for agentic MM-RAG with long, step-wise annotated reasoning chains spanning five representative reasoning structures. Each example specifies sub-questions, retrieval modalities, supporting facts, and intermediate answers, with fidelity ensured by HAVE (Hop-wise Attribution and Verification of Evidence), resulting in 3,333 high-quality examples averaging 3.7 hops. Beyond answer accuracy, MC-Search introduces new process-level metrics for reasoning quality, stepwise retrieval and planning accuracy. By developing a unified agentic MM-RAG pipeline, we benchmark six leading MLLMs and reveal systematic issues such as over- and under-retrieval and modality-misaligned planning. Finally, we introduce Search-Align, a process-supervised fine-tuning framework leveraging verified reasoning chains, showing that our data not only enables faithful evaluation but also improves planning and retrieval fidelity in open-source MLLMs.

## Graph
- **Concepts:** [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00873v1)
