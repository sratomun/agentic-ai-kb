---
type: source
source_type: arxiv
depth: abstract
title: "Disambiguate First, Parse Later: Generating Interpretations for Ambiguity Resolution in Semantic Parsing"
authors: Irina Saparina, Mirella Lapata (Edinburgh)
url: https://arxiv.org/abs/2502.18448
date: 2025-02-25
venue: Findings of ACL 2025
tags: [intent-grounding, intent-understanding, data-query-agents, arxiv, semantic-layer-corpus]
---

# Disambiguate First, Parse Later: Generating Interpretations for Ambiguity Resolution in Semantic Parsing

**arXiv:** [2502.18448](https://arxiv.org/abs/2502.18448) · 2025-02-25 · Findings of ACL 2025
**Authors:** Irina Saparina, Mirella Lapata (Edinburgh)

> Abstract-tier note (extended-search corpus, not in the local agents-centric census). Part of the intent-grounding / semantic-layer thread (2026-06-23).

## Abstract
Handling ambiguity and underspecification is an important challenge in natural language interfaces, particularly for tasks like text-to-SQL semantic parsing. We propose a modular approach that resolves ambiguity at the natural-language level before mapping to SQL logical forms: LLMs parse unambiguous utterances well but show strong biases on ambiguous ones, typically predicting only the preferred interpretation. The method first generates the preferred disambiguations, then applies a specialized infilling model to identify and generate the missing interpretations, trained with an annotation method that uses SQL execution to validate distinct meanings. The approach improves interpretation coverage and generalizes across datasets with different annotation styles, database structures, and ambiguity types.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[intent-understanding|Intent understanding]] · [[data-query-agents|Data-query agents]]
- **Entities:** [[ambrosia]]
