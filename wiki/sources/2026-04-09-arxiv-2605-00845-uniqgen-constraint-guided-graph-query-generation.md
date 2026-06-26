---
type: source
source_type: arxiv
depth: abstract
title: "Graph Query Generation with Constraint-guided Large Language Agents (UniQGen)"
authors: Mengying Wang et al.
url: https://arxiv.org/abs/2605.00845
date: 2026-04-09
venue: arXiv 2026
tags: [text-to-cypher, semantic-parsing, knowledge-graph, arxiv, text-to-cypher-corpus]
---

# Graph Query Generation with Constraint-guided Large Language Agents (UniQGen)

**arXiv:** [2605.00845](https://arxiv.org/abs/2605.00845) · 2026-04-09 · arXiv 2026
**Authors:** Mengying Wang et al.

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
Knowledge Graph Question Answering (KGQA) has advanced through structured query generation, yet most efforts target RDF/SPARQL, leaving Cypher and property graphs underexplored, despite increasing demand for unified KGQA in industry settings. We propose UniQGen, a novel constraint-based framework that employs LLM agents to dynamically extract and refine representative graph query clauses into executable, intent-aligned graph queries across query languages. The foundation of our method is a variant of Chase & Backchase, a family of algorithms for query optimization and reformulation. We extend Chase & Backchase with a dynamic reasoning process over query constraints that also interact with LLMs for query quality estimation. With a Cypher-supported Freebase graph deployed on Amazon Neptune, we extensively evaluate our approach on popular KGQA benchmarks (GraphQ, GrailQA, and WebQSP). We demonstrate that UniQGen outperforms state-of-the-art graph query generation techniques in both accuracy and efficiency, with F1 gains of 31.6% on GraphQ and 4.9% on GrailQA. Unlike prior methods, our framework does not require fine-tuning for schema matching, making it more extensible to schema-less graphs and semantics in query workloads, and is more suitable for enterprise-grade KGQA.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing|Semantic parsing]] · [[knowledge-graph|Knowledge graph]]
- **Entities:** [[cypher]]
