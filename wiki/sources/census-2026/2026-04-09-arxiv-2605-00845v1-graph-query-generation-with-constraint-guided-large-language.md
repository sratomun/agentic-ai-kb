---
type: source
source_type: arxiv
title: "Graph Query Generation with Constraint-guided Large Language Agents"
authors: Mengying Wang, Nicolaas Jedema, Rahul Pandey, RaviKiran Krishnan et al.
url: https://arxiv.org/abs/2605.00845v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.DB
tags: [knowledge-graph, agent-evaluation, arxiv, auto-ingested]
---

# Graph Query Generation with Constraint-guided Large Language Agents

**arXiv:** [2605.00845v1](https://arxiv.org/abs/2605.00845v1) · 2026-04-09 · cs.DB
**Authors:** Mengying Wang, Nicolaas Jedema, Rahul Pandey, RaviKiran Krishnan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Knowledge Graph Question Answering (KGQA) has advanced through structured query generation, yet most efforts target RDF/SPARQL, leaving Cypher and property graphs underexplored, despite increasing demand for unified KGQA in industry settings. We propose UniQGen, a novel constraint-based framework that employs LLM agents to dynamically extract and refine representative graph query clauses into executable, intent-aligned graph queries across query languages. The foundation of our method is a variant of Chase & Backchase, a family of algorithms for query optimization and reformulation. We extend Chase & Backchase with a dynamic reasoning process over query constraints that also interact with LLMs for query quality estimation. With a Cypher-supported Freebase graph deployed on Amazon Neptune, we extensively evaluate our approach on popular KGQA benchmarks (GraphQ, GrailQA, and WebQSP). We demonstrate that UniQGen outperforms state-of-the-art graph query generation techniques in both accuracy and efficiency, with F1 gains of 31.6% on GraphQ and 4.9% on GrailQA. Unlike prior methods, our framework does not require fine-tuning for schema matching, making it more extensible to schema-less graphs and semantics in query workloads, and is more suitable for enterprise-grade KGQA. We release Cypher outputs and a Neptune-ready Freebase snapshot to support reproducible, cross-language KGQA research.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.00845v1)
