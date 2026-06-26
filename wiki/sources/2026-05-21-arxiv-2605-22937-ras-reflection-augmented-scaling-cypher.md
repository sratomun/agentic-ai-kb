---
type: source
source_type: arxiv
depth: abstract
title: "RAS: Reflection-Augmented Scaling with In-Context Learning for Executable Cypher Query Generation"
authors: Minseok Jung, Abhas Ricky, Muhammad Rameez Chatni
url: https://arxiv.org/abs/2605.22937
date: 2026-05-21
venue: arXiv 2026
tags: [text-to-cypher, semantic-parsing, arxiv, text-to-cypher-corpus]
---

# RAS: Reflection-Augmented Scaling with In-Context Learning for Executable Cypher Query Generation

**arXiv:** [2605.22937](https://arxiv.org/abs/2605.22937) · 2026-05-21 · arXiv 2026
**Authors:** Minseok Jung, Abhas Ricky, Muhammad Rameez Chatni

> Abstract-tier note (extended-search corpus). Part of the text-to-Cypher / semantic-parsing thread (2026-06-23).

## Abstract
Inference-time scaling can reduce errors in structured query generation, but methods to allocate the compute for query code generation remains underexplored. We study Text2Cypher, where language models generate Cypher queries that execute against property graph databases. Non-executable queries constitute a distinct syntactic failure separate from semantic inaccuracy: a syntax error triggers a system-generated error message from the database. These error messages are typically discarded at inference time rather than leveraged through in-context learning (ICL). We compare two inference methods: Independent Scaling (IS), which performs memoryless resampling, and Reflection-Augmented Scaling (RAS), which conditions each new attempt on prior execution feedback via ICL. Across three Neo4j datasets and five code-specialized language models, RAS reduces the Query Execution Error Rate by 41--50% at n=5, outperforming IS at 32--38%. Execution errors are not merely failures to discard but actionable feedback, and structuring inference-time compute around them is a more efficient path to executability than scaling independent samples.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing|Semantic parsing]]
- **Entities:** [[cypher]]
