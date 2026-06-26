---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Hypergraph Enterprise Agentic Reasoner over Heterogeneous Business Systems (HEAR)"
authors: SUPCON
url: https://arxiv.org/abs/2605.14259
date: 2026-05-14
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, mediated-architecture, knowledge-graph, obda, multi-agent-systems]
---

# Hypergraph Enterprise Agentic Reasoner over Heterogeneous Business Systems (HEAR)

**arXiv [2605.14259](https://arxiv.org/abs/2605.14259)** · 2026-05-14 · SUPCON

**Significance.** The enterprise instantiation of the mediated model: a **Virtual Knowledge Graph** over BPM/ERP/SRM/WMS (data in-place via declarative mappings) plus n-ary business rules, reasoned over by an LLM. The on-the-ground proof for [[mediated-semantic-architecture]].

## Abstract
HEAR builds a Stratified Hypergraph Ontology: a Graph Layer virtualises provenance-aware data interfaces (each node = a semantic view of a DB table or API endpoint, data staying in-place — the Virtual Knowledge Graph paradigm), and a Hyperedge Layer encodes n-ary business rules as natural-language "soft axioms" (declarative facts + procedural workflows). An LLM runs an evidence-driven reasoning loop over ontology tools, no retraining.

## From the paper (full-text, via subagent)
**Contribution / method.** [[virtual-knowledge-graph|VKG]]-based data layer + hypergraph business rules; tools include BFS topology exploration and Aho-Corasick + dense (BGE) / sparse (BM25) hyperedge retrieval. Mediates across four real systems (BPM, ERP, SRM, WMS); backbone GPT-5, ≤50 tool turns.
**Results.** 20 synced tables; OF-BRCA (95 root-cause, binary) and OF-General (160, three-way). **OF-BRCA: HEAR Complete 94.7%** (6.3 turns / 38.1K tokens) vs HEAR-Declarative 74.2%, Table-RAG 52.6%, Table-list 51.5%, CSR-RAG 11.3%; removing procedural hyperedges costs **−20.5 pts** and inflates cost to 14.9 turns / 179.3K tokens. Backbones: GPT-5 94.7%, DeepSeek-3.2 93.8%, **Qwen-3.5-27B 92.7%** (open-weight near-parity), Qwen-Next-80B collapses to 45.4%. Practical: 200 blockages = 20 person-days manual → under 10 hours.
**Takeaway.** Virtualise enterprise systems as a graph (don't ETL), encode business rules as retrievable hyperedges, and let an agent reason over them — near-frontier accuracy from an open 27B model. Caveat: single proprietary SUPCON deployment, NDA, not independently reproducible.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[knowledge-graph]] · [[multi-agent-systems]]
- **Entities:** [[virtual-knowledge-graph]] · [[ontology-based-data-access]]
- **Raw:** full-text (alphaXiv, read via subagent) 2026-06-23
