---
type: source
source_type: arxiv
title: "From Conflict to Consensus: Boosting Medical Reasoning via Multi-Round Agentic RAG"
authors: Wenhao Wu, Zhentao Tang, Yafu Li, Shixiong Kai et al.
url: https://arxiv.org/abs/2603.03292v3
date: 2026-02-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [clinical-agents, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# From Conflict to Consensus: Boosting Medical Reasoning via Multi-Round Agentic RAG

**arXiv:** [2603.03292v3](https://arxiv.org/abs/2603.03292v3) · 2026-02-06 · cs.CL
**Authors:** Wenhao Wu, Zhentao Tang, Yafu Li, Shixiong Kai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) exhibit high reasoning capacity in medical question-answering, but their tendency to produce hallucinations and outdated knowledge poses critical risks in healthcare fields. While Retrieval-Augmented Generation (RAG) mitigates these issues, existing methods rely on noisy token-level signals and lack the multi-round refinement required for complex reasoning. In this paper, we propose MA-RAG (Multi-Round Agentic RAG), a framework that facilitates test-time scaling for complex medical reasoning by iteratively evolving both external evidence and internal reasoning history within an agentic refinement loop. At each round, the agent transforms semantic conflict among candidate responses into actionable queries to retrieve external evidence, while optimizing history reasoning traces to mitigate long-context degradation. MA-RAG extends the self-consistency principle by leveraging the lack of consistency as a proactive signal for multi-round agentic reasoning and retrieval, and mirrors a boosting mechanism that iteratively minimizes the residual error toward a stable, high-fidelity medical consensus. Extensive evaluations across 7 medical Q&A benchmarks show that MA-RAG consistently surpasses competitive inference-time scaling and RAG baselines, delivering substantial +6.8 points on average accuracy over the backbone model. Our code is available at https://github.com/NJU-RL/MA-RAG.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.03292v3)
