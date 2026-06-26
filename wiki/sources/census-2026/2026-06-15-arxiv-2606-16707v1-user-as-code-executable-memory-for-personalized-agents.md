---
type: source
source_type: arxiv
title: "User as Code: Executable Memory for Personalized Agents"
authors: Bojie Li
url: https://arxiv.org/abs/2606.16707v1
date: 2026-06-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.AI
tags: [knowledge-graph, agent-security, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# User as Code: Executable Memory for Personalized Agents

**arXiv:** [2606.16707v1](https://arxiv.org/abs/2606.16707v1) · 2026-06-15 · cs.AI
**Authors:** Bojie Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
A personalized AI agent needs a user memory: a persistent model of who the user is, built across many conversations and consulted on each new one. Today this memory is almost always stored as unstructured text, a knowledge graph, or a flat store of facts, and consulted by retrieval -- fetching the entries most similar to the current request. Such "bag-of-facts" memory recalls individual facts well, but because storing a fact and acting on it are separate steps, it struggles to resolve contradictions, aggregate over many records, or enforce rules. We argue that user memory should instead be executable. We introduce User as Code (UaC), a paradigm in which an agent's model of a user is a living software project: typed Python objects hold the user's state and ordinary Python functions encode the rules that govern it, so representing and reasoning about the user happen in one medium an interpreter can run. The enabling mechanism is a two-phase pipeline: an append-only log that never discards a fact, periodically checkpointed into typed code. This changes what memory can do. On standard long-term conversation benchmarks, UaC matches both a full-context upper bound and the strongest prior memory systems on recall (78.8% on LOCOMO). Its advantage emerges where representation matters most. On aggregate questions over a user's history -- "how many international trips did I take last year?" -- retrieval-based memory collapses (6-43%) while UaC stays near-perfect (99%), because the answer is a one-line computation over typed state rather than a search over text. And because its rules execute deterministically whenever the state changes, UaC can surface unsolicited, safety-critical alerts -- such as a newly prescribed drug that conflicts with an allergy recorded months earlier -- a capability query-driven memory cannot provide.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.16707v1)
