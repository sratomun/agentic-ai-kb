---
type: source
source_type: arxiv
title: "BADGER: Bridging Agentic and Deterministic Evaluation for Generative Enterprise Reasoning"
authors: Shannon Serrao, Soumitra Chatterjee, Dorina Strori, Abhishek Sharma et al.
url: https://arxiv.org/abs/2606.02109v1
date: 2026-06-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [data-query-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# BADGER: Bridging Agentic and Deterministic Evaluation for Generative Enterprise Reasoning

**arXiv:** [2606.02109v1](https://arxiv.org/abs/2606.02109v1) · 2026-06-01 · cs.AI
**Authors:** Shannon Serrao, Soumitra Chatterjee, Dorina Strori, Abhishek Sharma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enterprise AI systems that translate natural language into SQL queries and orchestrate multi-step agentic reasoning pipelines require evaluation approaches fundamentally different from academic benchmarks. Spider and BIRD established execution-accuracy protocols; G-Eval and RAGAS advanced LLM-based assessment; and recent work such as Spider 2.0, BEAVER, and BIRD-Interact has begun to address enterprise and agentic dimensions. No single framework unifies text-to-SQL assessment with agentic behavior evaluation into a production-grade pipeline calibrated against human expert judgment. We present BADGER, developed at Merkle, a unified evaluation framework integrating text-to-SQL assessment with agentic behavior evaluation. BADGER offers three contributions. First, LLM-assisted SQL component extraction extending Spider methodology to handle CTE-heavy, dialect-specific SQL. Second, a hybrid execution accuracy metric (Hybrid-EX) resolving column-aliasing and numeric-tolerance brittleness by using an LLM to infer structural alignments before deterministic cell-level scoring. Validated on 150 human-annotated industry queries, Hybrid-EX achieves Cohen's kappa=0.717 [95% CI: 0.600-0.822] (Substantial agreement) and 87.3% balanced accuracy, outperforming all six competing frameworks (Delta-kappa: 0.322-0.502, all p<=0.001). Third, an enterprise agentic evaluation suite assembling RAGAS, G-Eval, and agent benchmark metrics into a unified pipeline; Excess Tool Usage is the sole novel element. BADGER runs entirely within the client's governed data environment, supports configurable LLM judge backends, and enables rapid prototyping of client-specific judges and metrics, serving as a continuous evaluation backbone rather than a one-time quality gate.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]] · [[spider-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.02109v1)
