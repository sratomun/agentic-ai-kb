---
type: source
source_type: arxiv
depth: abstract
title: "AMBROSIA: A Benchmark for Parsing Ambiguous Questions into Database Queries"
authors: Irina Saparina, Mirella Lapata (Edinburgh)
url: https://arxiv.org/abs/2406.19073
date: 2024-06-27
venue: NeurIPS 2024 D&B (Spotlight)
tags: [intent-grounding, intent-understanding, data-query-agents, arxiv, semantic-layer-corpus]
---

# AMBROSIA: A Benchmark for Parsing Ambiguous Questions into Database Queries

**arXiv:** [2406.19073](https://arxiv.org/abs/2406.19073) · 2024-06-27 · NeurIPS 2024 D&B (Spotlight)
**Authors:** Irina Saparina, Mirella Lapata (Edinburgh)

> Abstract-tier note (extended-search corpus, not in the local agents-centric census). Part of the intent-grounding / semantic-layer thread (2026-06-23).

## Abstract
Practical semantic parsers are expected to understand user utterances and map them to executable programs, even when these are ambiguous. We introduce a new benchmark, AMBROSIA, which we hope will inform and inspire the development of text-to-SQL parsers capable of recognizing and interpreting ambiguous requests. Our dataset contains questions showcasing three different types of ambiguity (scope ambiguity, attachment ambiguity, and vagueness), their interpretations, and corresponding SQL queries. In each case, the ambiguity persists even when the database context is provided. This is achieved through a novel approach that involves controlled generation of databases from scratch. We benchmark various LLMs on AMBROSIA, revealing that even the most advanced models struggle to identify and interpret ambiguity in questions.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[intent-understanding|Intent understanding]] · [[data-query-agents|Data-query agents]]
- **Entities:** [[ambrosia]]
