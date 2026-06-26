---
type: source
source_type: arxiv
title: "Knowledge Graphs as the Missing Data Layer for LLM-Based Industrial Asset Operations"
authors: Madhulatha Mandarapu, Sandeep Kunkunuru
url: https://arxiv.org/abs/2605.26874v2
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 6
primary: cs.DB
tags: [knowledge-graph, multi-agent-systems, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# Knowledge Graphs as the Missing Data Layer for LLM-Based Industrial Asset Operations

**arXiv:** [2605.26874v2](https://arxiv.org/abs/2605.26874v2) · 2026-05-26 · cs.DB
**Authors:** Madhulatha Mandarapu, Sandeep Kunkunuru

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based agents for industrial asset operations show limited accuracy when reasoning over flat document stores. AssetOpsBench (KDD 2026) establishes that GPT-4 agents achieve 65% on 139 industrial maintenance scenarios, and compares LLM orchestration paradigms (Agent-As-Tool vs. Plan-Execute) on a fixed data layer. We ask the orthogonal question: how much does the data model behind the tools matter? We treat a typed knowledge graph as a grounding substrate and route each question by how it is best answered: (i) LLM-generated Cypher for structured retrieval, which lifts the same GPT-4 model from 65% to 82-83%; (ii) native graph and optimization primitives, with no LLM, reaching 99% on graph-answerable scenarios; and (iii) generation-augmented knowledge (GAK) for answers absent from the data -- the engine's agent materializes the missing facts as provenance-tagged graph nodes, then answers. A recurring theme is inverted LLM usage: we constrain the LLM to query generation or one-shot enrichment from a typed schema and let the graph execute deterministically. On the 88 real AssetOpsBench failure-mode scenarios the benchmark itself flags non-deterministic -- ten equipment types absent from the graph -- GAK lifts answerability from zero to 100% of equipment types and answers 81.8% of scenarios, every materialized fact tagged source:LLM-derived for auditability. We also contribute 40 graph-native scenarios. For structured operational domains the data layer -- not the LLM orchestration -- is the primary lever, and a typed knowledge graph serves as a grounding substrate between raw industrial data and LLM reasoning.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26874v2)
