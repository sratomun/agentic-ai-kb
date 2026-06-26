---
type: source
source_type: arxiv
depth: abstract
title: "OmniRetrieval: Unified Retrieval across Heterogeneous Knowledge Sources"
authors: Jinheon Baek et al.
url: https://arxiv.org/abs/2605.29250
date: 2026-05-28
venue: arXiv 2026
tags: [mediated-semantic-architecture, semantic-parsing, agentic-rag, arxiv, mediated-architecture-corpus]
---

# OmniRetrieval: Unified Retrieval across Heterogeneous Knowledge Sources

**arXiv:** [2605.29250](https://arxiv.org/abs/2605.29250) · 2026-05-28 · arXiv 2026
**Authors:** Jinheon Baek et al.

> Abstract-tier note (extended-search corpus). Part of the mediated-semantic-architecture thread (2026-06-23).

## Abstract
Real-world information needs require access to structurally diverse knowledge sources, from unstructured text and relational tables to knowledge graphs and property graphs. Existing retrievers, however, operate over one source at a time under a fixed query language, leaving the broader landscape of available knowledge fragmented behind incompatible interfaces. A natural attempt at unification would collapse these sources into a shared space, but this erases the structural affordances (such as schemas, ontologies, compositional operators) that give each source its expressive power. Effective retrieval over diverse knowledge, therefore, requires not homogenization but an overarching layer that meets each source on its own terms. To achieve this, we present OmniRetrieval, a framework that takes any natural-language query, identifies appropriate knowledge sources, and dispatches source-native queries to their native execution engines. Across an extensive benchmark spanning 13 datasets and 309 distinct knowledge bases over text, relational, and graph-structured sources, OmniRetrieval exceeds single-source baselines, demonstrating that it can serve as a general-purpose interface to the heterogeneous sources while preserving the structural distinctions that make each source valuable.

## Graph
- **Concepts:** [[mediated-semantic-architecture|Mediated semantic architecture]] · [[semantic-parsing|Semantic parsing]] · [[agentic-rag|Agentic RAG]]
- **Entities:** [[text-to-query-wrapper]]
