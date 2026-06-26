---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "SLM-Based Agentic AI with P-C-G: Optimized for Korean Tool Use"
authors: Changhyun Jeon et al.
url: https://arxiv.org/abs/2509.19369v1
date: 2025-09-19
score: 21
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, coding-agents]
---

# SLM-Based Agentic AI with P-C-G: Optimized for Korean Tool Use

**arXiv:** [2509.19369v1](https://arxiv.org/abs/2509.19369v1) · 2025-09-19 · cs.CL
**Authors:** Changhyun Jeon et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We propose a small-scale language model (SLM) based agent architecture, Planner-Caller-Generator (P-C-G), optimized for Korean tool use. P-C-G separates planning, calling, and generation by role: the Planner produces an initial batch plan with limited on-demand replanning; the Caller returns a normalized call object after joint schema-value validation; and the Generator integrates tool outputs to produce the final answer. We apply a Korean-first value policy to reduce execution failures caused by frequent Korean-to-English code switching in Korean settings. Evaluation assumes Korean queries and Korean tool/parameter specifications; it covers single-chain, multi-chain, missing-parameters, and missing-functions scenarios, and is conducted via an LLM-as-a-Judge protocol averaged over five runs under a unified I/O interface. Results show that P-C-G delivers competitive tool-use accuracy and end-to-end quality while reducing tokens and maintaining acceptable latency, indicating that role-specialized SLMs are a cost-effective alternative for Korean tool-use agents.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2509.19369v1)
