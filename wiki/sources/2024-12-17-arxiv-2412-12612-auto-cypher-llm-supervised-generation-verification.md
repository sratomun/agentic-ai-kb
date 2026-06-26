---
type: source
source_type: arxiv
depth: abstract
title: "Auto-Cypher: Improving LLMs on Cypher generation via LLM-supervised generation-verification framework"
authors: Aman Tiwari et al. (ServiceNow)
url: https://arxiv.org/abs/2412.12612
date: 2024-12-17
venue: NAACL 2025
tags: [text-to-cypher, semantic-parsing, synthetic-data, arxiv, text-to-cypher-corpus]
---

# Auto-Cypher: Improving LLMs on Cypher generation via LLM-supervised generation-verification framework

**arXiv:** [2412.12612](https://arxiv.org/abs/2412.12612) · 2024-12-17 · NAACL 2025
**Authors:** Aman Tiwari et al. (ServiceNow)

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
Graph databases like Neo4j are gaining popularity for handling complex, interconnected data, over traditional relational databases in modeling and querying relationships. While translating natural language into SQL queries is well-researched, generating Cypher queries for Neo4j remains relatively underexplored. In this work, we present an automated, LLM-Supervised, pipeline to generate high-quality synthetic data for Text2Cypher. Our Cypher data generation pipeline introduces LLM-As-Database-Filler, a novel strategy for ensuring Cypher query correctness, thus resulting in high quality generations. Using our pipeline, we generate high quality Text2Cypher data - SynthCypher containing 29.8k instances across various domains and queries with varying complexities. Training open-source LLMs like LLaMa-3.1-8B, Mistral-7B, and QWEN-7B on SynthCypher results in performance gains of up to 40% on the Text2Cypher test split and 30% on the SPIDER benchmark, adapted for graph databases.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing|Semantic parsing]] · [[synthetic-data|Synthetic data]]
- **Entities:** [[cypher]]
