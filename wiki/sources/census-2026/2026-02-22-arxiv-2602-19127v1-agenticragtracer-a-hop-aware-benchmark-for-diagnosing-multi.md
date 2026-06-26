---
type: source
source_type: arxiv
title: "AgenticRAGTracer: A Hop-Aware Benchmark for Diagnosing Multi-Step Retrieval Reasoning in Agentic RAG"
authors: Qijie You, Wenkai Yu, Wentao Zhang
url: https://arxiv.org/abs/2602.19127v1
date: 2026-02-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [clinical-agents, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# AgenticRAGTracer: A Hop-Aware Benchmark for Diagnosing Multi-Step Retrieval Reasoning in Agentic RAG

**arXiv:** [2602.19127v1](https://arxiv.org/abs/2602.19127v1) · 2026-02-22 · cs.CL
**Authors:** Qijie You, Wenkai Yu, Wentao Zhang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
With the rapid advancement of agent-based methods in recent years, Agentic RAG has undoubtedly become an important research direction. Multi-hop reasoning, which requires models to engage in deliberate thinking and multi-step interaction, serves as a critical testbed for assessing such capabilities. However, existing benchmarks typically provide only final questions and answers, while lacking the intermediate hop-level questions that gradually connect atomic questions to the final multi-hop query. This limitation prevents researchers from analyzing at which step an agent fails and restricts more fine-grained evaluation of model capabilities. Moreover, most current benchmarks are manually constructed, which is both time-consuming and labor-intensive, while also limiting scalability and generalization. To address these challenges, we introduce AgenticRAGTracer, the first Agentic RAG benchmark that is primarily constructed automatically by large language models and designed to support step-by-step validation. Our benchmark spans multiple domains, contains 1,305 data points, and has no overlap with existing mainstream benchmarks. Extensive experiments demonstrate that even the best large language models perform poorly on our dataset. For instance, GPT-5 attains merely 22.6\% EM accuracy on the hardest portion of our dataset. Hop-aware diagnosis reveals that failures are primarily driven by distorted reasoning chains -- either collapsing prematurely or wandering into over-extension. This highlights a critical inability to allocate steps consistent with the task's logical structure, providing a diagnostic dimension missing in traditional evaluations. We believe our work will facilitate research in Agentic RAG and inspire further meaningful progress in this area. Our code and data are available at https://github.com/YqjMartin/AgenticRAGTracer.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.19127v1)
