---
type: source
source_type: arxiv
title: "Beyond Fine-Tuning: Robust Food Entity Linking under Ontology Drift with FoodOntoRAG"
authors: Jan Drole, Ana Gjorgjevikj, Barbara Korouši'c Seljak, Tome Eftimov
url: https://arxiv.org/abs/2603.09758v1
date: 2026-03-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 1
primary: cs.CL
tags: [knowledge-graph, agent-reliability, agent-security, arxiv, auto-ingested]
---

# Beyond Fine-Tuning: Robust Food Entity Linking under Ontology Drift with FoodOntoRAG

**arXiv:** [2603.09758v1](https://arxiv.org/abs/2603.09758v1) · 2026-03-10 · cs.CL
**Authors:** Jan Drole, Ana Gjorgjevikj, Barbara Korouši'c Seljak, Tome Eftimov

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Standardizing food terms from product labels and menus into ontology concepts is a prerequisite for trustworthy dietary assessment and safety reporting. The dominant approach to Named Entity Linking (NEL) in the food and nutrition domains fine-tunes Large Language Models (LLMs) on task-specific corpora. Although effective, fine-tuning incurs substantial computational cost, ties models to a particular ontology snapshot (i.e., version), and degrades under ontology drift. This paper presents FoodOntoRAG, a model- and ontology-agnostic pipeline that performs few-shot NEL by retrieving candidate entities from domain ontologies and conditioning an LLM on structured evidence (food labels, synonyms, definitions, and relations). A hybrid lexical--semantic retriever enumerates candidates; a selector agent chooses a best match with rationale; a separate scorer agent calibrates confidence; and, when confidence falls below a threshold, a synonym generator agent proposes reformulations to re-enter the loop. The pipeline approaches state-of-the-art accuracy while revealing gaps and inconsistencies in existing annotations. The design avoids fine-tuning, improves robustness to ontology evolution, and yields interpretable decisions through grounded justifications.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.09758v1)
