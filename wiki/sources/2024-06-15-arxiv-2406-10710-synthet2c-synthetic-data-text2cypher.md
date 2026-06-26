---
type: source
source_type: arxiv
depth: abstract
title: "SyntheT2C: Generating Synthetic Data for Fine-Tuning Large Language Models on the Text2Cypher Task"
authors: Zijie Zhong et al.
url: https://arxiv.org/abs/2406.10710
date: 2024-06-15
venue: COLING 2025
tags: [text-to-cypher, semantic-parsing, synthetic-data, knowledge-graph, arxiv, text-to-cypher-corpus]
---

# SyntheT2C: Generating Synthetic Data for Fine-Tuning Large Language Models on the Text2Cypher Task

**arXiv:** [2406.10710](https://arxiv.org/abs/2406.10710) · 2024-06-15 · COLING 2025
**Authors:** Zijie Zhong et al.

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
Integrating Large Language Models (LLMs) with existing Knowledge Graph (KG) databases presents a promising avenue for enhancing LLMs' efficacy and mitigating their "hallucinations". Given that most KGs reside in graph databases accessible solely through specialized query languages (e.g., Cypher), it is critical to connect LLMs with KG databases by automating the translation of natural language into Cypher queries (termed as "Text2Cypher" task). Prior efforts tried to bolster LLMs' proficiency in Cypher generation through Supervised Fine-Tuning (SFT). However, these explorations are hindered by the lack of annotated datasets of Query-Cypher pairs, resulting from the labor-intensive and domain-specific nature of such annotation. In this study, we propose SyntheT2C, a methodology for constructing a synthetic Query-Cypher pair dataset, comprising two distinct pipelines: (1) LLM-based prompting and (2) template-filling. SyntheT2C is applied to two medical KG databases, culminating in the creation of a synthetic dataset, MedT2C. Comprehensive experiments demonstrate that the MedT2C dataset effectively enhances the performance of backbone LLMs on Text2Cypher task via SFT.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing|Semantic parsing]] · [[synthetic-data|Synthetic data]] · [[knowledge-graph|Knowledge graph]]
- **Entities:** [[cypher]]
