---
type: source
source_type: arxiv
title: "Blue Data Intelligence Layer: Streaming Data and Agents for Multi-source Multi-modal Data-Centric Applications"
authors: Moin Aminnaseri, Farima Fatahi Bayat, Nikita Bhutani, Jean-Flavien Bussotti et al.
url: https://arxiv.org/abs/2604.15233v1
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [data-query-agents, multi-agent-systems, arxiv, auto-ingested]
---

# Blue Data Intelligence Layer: Streaming Data and Agents for Multi-source Multi-modal Data-Centric Applications

**arXiv:** [2604.15233v1](https://arxiv.org/abs/2604.15233v1) · 2026-04-16 · cs.AI
**Authors:** Moin Aminnaseri, Farima Fatahi Bayat, Nikita Bhutani, Jean-Flavien Bussotti et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
NL2SQL systems aim to address the growing need for natural language interaction with data. However, real-world information rarely maps to a single SQL query because (1) users express queries iteratively (2) questions often span multiple data sources beyond the closed-world assumption of a single database, and (3) queries frequently rely on commonsense or external knowledge. Consequently, satisfying realistic data needs require integrating heterogeneous sources, modalities, and contextual data. In this paper, we present Blue's Data Intelligence Layer (DIL) designed to support multi-source, multi-modal, and data-centric applications. Blue is a compound AI system that orchestrates agents and data for enterprise settings. DIL serves as the data intelligence layer for agentic data processing, to bridge the semantic gap between user intent and available information by unifying structured enterprise data, world knowledge accessible through LLMs, and personal context obtained through interaction. At the core of DIL is a data registry that stores metadata for diverse data sources and modalities to enable both native and natural language queries. DIL treats LLMs, the Web, and the User as source 'databases', each with their own query interface, elevating them to first-class data sources. DIL relies on data planners to transform user queries into executable query plans. These plans are declarative abstractions that unify relational operators with other operators spanning multiple modalities. DIL planners support decomposition of complex requests into subqueries, retrieval from diverse sources, and finally reasoning and integration to produce final results. We demonstrate DIL through two interactive scenarios in which user queries dynamically trigger multi-source retrieval, cross-modal reasoning, and result synthesis, illustrating how compound AI systems can move beyond single database NL2SQL.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.15233v1)
