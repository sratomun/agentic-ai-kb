---
type: source
source_type: arxiv
title: "Aggregation Queries over Unstructured Text: Benchmark and Agentic Method"
authors: Haojia Zhu, Qinyuan Xu, Haoyu Li, Yuxi Liu et al.
url: https://arxiv.org/abs/2602.01355v2
date: 2026-02-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [data-query-agents, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Aggregation Queries over Unstructured Text: Benchmark and Agentic Method

**arXiv:** [2602.01355v2](https://arxiv.org/abs/2602.01355v2) · 2026-02-01 · cs.AI
**Authors:** Haojia Zhu, Qinyuan Xu, Haoyu Li, Yuxi Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Aggregation query over free text is a long-standing yet underexplored problem. Unlike ordinary question answering, aggregate queries require exhaustive evidence collection and systems are required to "find all," not merely "find one." Existing paradigms such as Text-to-SQL and Retrieval-Augmented Generation fail to achieve this completeness. In this work, we formalize entity-level aggregation querying over text in a corpus-bounded setting with strict completeness requirement. To enable principled evaluation, we introduce AGGBench, a benchmark designed to evaluate completeness-oriented aggregation under realistic large-scale corpus. To accompany the benchmark, we propose DFA (Disambiguation--Filtering--Aggregation), a modular agentic baseline that decomposes aggregation querying into interpretable stages and exposes key failure modes related to ambiguity, filtering, and aggregation. Empirical results show that DFA consistently improves aggregation evidence coverage over strong RAG and agentic baselines. The data and code are available in \href{https://anonymous.4open.science/r/DFA-A4C1}.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.01355v2)
