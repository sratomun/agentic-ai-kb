---
type: source
source_type: arxiv
title: "Agentic Multi-Source Grounding for Enhanced Query Intent Understanding: A DoorDash Case Study"
authors: Emmanuel Aboah Boateng, Kyle MacDonald, Akshad Viswanathan et al.
url: https://arxiv.org/abs/2603.01486v2
date: 2026-03-02
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [intent-understanding, intent-routing, agentic-rag, arxiv, auto-ingested]
---

# Agentic Multi-Source Grounding for Enhanced Query Intent Understanding: A DoorDash Case Study

**arXiv:** [2603.01486v2](https://arxiv.org/abs/2603.01486v2) · 2026-03-02 · cs.AI
**Authors:** Emmanuel Aboah Boateng, Kyle MacDonald, Akshad Viswanathan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
Accurately mapping user queries to business categories is a fundamental Information Retrieval challenge for multi-category marketplaces, where context-sparse queries such as "Wildflower" exhibit intent ambiguity, simultaneously denoting a restaurant chain, a retail product, and a floral item. Traditional classifiers force a winner-takes-all assignment, while general-purpose LLMs hallucinate unavailable inventory. We introduce an Agentic Multi-Source Grounded system that addresses both failure modes by grounding LLM inference in (i) a staged catalog entity retrieval pipeline and (ii) an agentic web-search tool invoked autonomously for cold-start queries. Rather than predicting a single label, the model emits an ordered multi-intent set, resolved by a configurable disambiguation layer that applies deterministic business policies and is designed for extensibility to personalization signals. This decoupled design generalizes across domains, allowing any marketplace to supply its own grounding sources and resolution rules without modifying the core architecture. Evaluated on DoorDash's multi-vertical search platform, the system achieves +10.9pp over the ungrounded LLM baseline and +4.6pp over the legacy production system. On long-tail queries, incremental ablations attribute +8.3pp to catalog grounding, +3.2pp to agentic web search grounding, and +1.5pp to dual intent disambiguation, yielding 90.7% accuracy (+13.0pp over baseline). The system is deployed in production, serving over 95% of daily search impressions, and establishes a generalizable paradigm for applications requiring foundation models grounded in proprietary context and real-time web knowledge to resolve ambiguous, context-sparse decision problems at scale.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[intent-routing|Intent routing]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.01486v2)
