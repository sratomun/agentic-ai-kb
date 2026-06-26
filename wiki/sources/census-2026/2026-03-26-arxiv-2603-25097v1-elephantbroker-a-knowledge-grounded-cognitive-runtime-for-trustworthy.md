---
type: source
source_type: arxiv
title: "ElephantBroker: A Knowledge-Grounded Cognitive Runtime for Trustworthy AI Agents"
authors: Cristian Lupascu, Alexandru Lupascu
url: https://arxiv.org/abs/2603.25097v1
date: 2026-03-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.AI
tags: [knowledge-graph, human-agent-interaction, agent-security, agent-memory, tool-use, arxiv, auto-ingested]
---

# ElephantBroker: A Knowledge-Grounded Cognitive Runtime for Trustworthy AI Agents

**arXiv:** [2603.25097v1](https://arxiv.org/abs/2603.25097v1) · 2026-03-26 · cs.AI
**Authors:** Cristian Lupascu, Alexandru Lupascu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model based agents increasingly operate in high stakes, multi turn settings where factual grounding is critical, yet their memory systems typically rely on flat key value stores or plain vector retrieval with no mechanism to track the provenance or trustworthiness of stored knowledge. We present ElephantBroker, an open source cognitive runtime that unifies a Neo4j knowledge graph with a Qdrant vector store through the Cognee SDK to provide durable, verifiable agent memory. The system implements a complete cognitive loop (store, retrieve, score, compose, protect, learn) comprising a hybrid five source retrieval pipeline, an eleven dimension competitive scoring engine for budget constrained context assembly, a four state evidence verification model, a five stage context lifecycle with goal aware assembly and continuous compaction, a six layer cheap first guard pipeline for safety enforcement, an AI firewall providing enforceable tool call interception and multi tier safety scanning, a nine stage consolidation engine that strengthens useful patterns while decaying noise, and a numeric authority model governing multi organization identity with hierarchical access control. Architectural validation through a comprehensive test suite of over 2,200 tests spanning unit, integration, and end to end levels confirms subsystem correctness. The modular design supports three deployment tiers, five profile presets with inheritance, multi gateway isolation, and a management dashboard for human oversight, enabling configurations from lightweight memory only agents to full cognitive runtimes with enterprise grade safety and auditability.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[human-agent-interaction|Human-agent interaction]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.25097v1)
