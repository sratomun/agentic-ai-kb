---
type: source
source_type: arxiv
title: "Clinical Knowledge Graph Construction and Evaluation with Multi-LLMs via Retrieval-Augmented Generation"
authors: Udiptaman Das, Krishnasai B. Atmakuri, Duy Ho, Chi Lee et al.
url: https://arxiv.org/abs/2601.01844v1
date: 2026-01-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agentic-rag, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Clinical Knowledge Graph Construction and Evaluation with Multi-LLMs via Retrieval-Augmented Generation

**arXiv:** [2601.01844v1](https://arxiv.org/abs/2601.01844v1) · 2026-01-05 · cs.AI
**Authors:** Udiptaman Das, Krishnasai B. Atmakuri, Duy Ho, Chi Lee et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) offer new opportunities for constructing knowledge graphs (KGs) from unstructured clinical narratives. However, existing approaches often rely on structured inputs and lack robust validation of factual accuracy and semantic consistency, limitations that are especially problematic in oncology. We introduce an end-to-end framework for clinical KG construction and evaluation directly from free text using multi-agent prompting and a schema-constrained Retrieval-Augmented Generation (KG-RAG) strategy. Our pipeline integrates (1) prompt-driven entity, attribute, and relation extraction; (2) entropy-based uncertainty scoring; (3) ontology-aligned RDF/OWL schema generation; and (4) multi-LLM consensus validation for hallucination detection and semantic refinement. Beyond static graph construction, the framework supports continuous refinement and self-supervised evaluation, enabling iterative improvement of graph quality. Applied to two oncology cohorts (PDAC and BRCA), our method produces interpretable, SPARQL-compatible, and clinically grounded knowledge graphs without relying on gold-standard annotations. Experimental results demonstrate consistent gains in precision, relevance, and ontology compliance over baseline methods.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.01844v1)
