---
type: source
source_type: arxiv
depth: abstract
title: "DBCopilot: Scaling Natural Language Querying to Massive Databases"
authors: Tianshu Wang et al.
url: https://arxiv.org/abs/2312.03463
date: 2023-12-06
venue: arXiv 2023
tags: [mediated-semantic-architecture, intent-routing, data-query-agents, arxiv, mediated-architecture-corpus]
---

# DBCopilot: Scaling Natural Language Querying to Massive Databases

**arXiv:** [2312.03463](https://arxiv.org/abs/2312.03463) · 2023-12-06 · arXiv 2023
**Authors:** Tianshu Wang et al.

> Abstract-tier note (extended-search corpus). Part of the mediated-semantic-architecture thread (2026-06-23).

## Abstract
The development of Natural Language Interfaces to Databases (NLIDBs) has been greatly advanced by the advent of large language models (LLMs), which provide an intuitive way to translate natural language (NL) questions into Structured Query Language (SQL) queries. While significant progress has been made in LLM-based NL2SQL, existing approaches face several challenges in real-world scenarios of natural language querying over massive databases. In this paper, we present DBCopilot, a framework that addresses these challenges by employing a compact and flexible copilot model for routing over massive databases. Specifically, DBCopilot decouples schema-agnostic NL2SQL into schema routing and SQL generation. This framework utilizes a single lightweight differentiable search index to construct semantic mappings for massive database schemata, and navigates natural language questions to their target databases and tables in a relation-aware joint retrieval manner. The routed schemata and questions are then fed into LLMs for effective SQL generation. Furthermore, DBCopilot introduces a reverse schema-to-question generation paradigm that can automatically learn and adapt the router over massive databases without manual intervention. Experimental results verify that DBCopilot is a scalable and effective solution for schema-agnostic NL2SQL, providing a significant advance in handling natural language querying over massive databases for NLIDBs.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[intent-routing|Intent routing]] · [[data-query-agents|Data-query agents]]
