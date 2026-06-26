---
type: source
source_type: arxiv
title: "A Reference Architecture for Agentic Hybrid Retrieval in Dataset Search"
authors: Riccardo Terrenzi, Phongsakon Mark Konrad, Tim Lukas Adam, Serkan Ayvaz
url: https://arxiv.org/abs/2604.16394v1
date: 2026-03-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.IR
tags: [agent-reliability, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# A Reference Architecture for Agentic Hybrid Retrieval in Dataset Search

**arXiv:** [2604.16394v1](https://arxiv.org/abs/2604.16394v1) · 2026-03-28 · cs.IR
**Authors:** Riccardo Terrenzi, Phongsakon Mark Konrad, Tim Lukas Adam, Serkan Ayvaz

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Ad hoc dataset search requires matching underspecified natural-language queries against sparse, heterogeneous metadata records, a task where typical lexical or dense retrieval alone falls short. We reposition dataset search as a software-architecture problem and propose a bounded, auditable reference architecture for agentic hybrid retrieval that combines BM25 lexical search with dense-embedding retrieval via reciprocal rank fusion (RRF), orchestrated by a large language model (LLM) agent that repeatedly plans queries, evaluates the sufficiency of results, and reranks candidates. To reduce the vocabulary mismatch between user intent and provider-authored metadata, we introduce an offline metadata augmentation step in which an LLM generates pseudo-queries for each dataset record, augmenting both retrieval indexes before query time. Two architectural styles are examined: a single ReAct agent and a multi-agent horizontal architecture with Feedback Control. Their quality-attribute tradeoffs are analyzed with respect to modifiability, observability, performance, and governance. An evaluation framework comprising seven system variants is defined to isolate the contribution of each architectural decision. The architecture is presented as an extensible reference design for the software architecture community, incorporating explicit governance tactics to bound and audit nondeterministic LLM components.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16394v1)
