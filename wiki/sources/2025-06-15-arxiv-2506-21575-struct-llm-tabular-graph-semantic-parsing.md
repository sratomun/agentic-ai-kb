---
type: source
source_type: arxiv
depth: abstract
title: "STRuCT-LLM: Unifying Tabular and Graph Reasoning with Reinforcement Learning for Semantic Parsing"
authors: Josefa Lia Stoisser et al. (Novo Nordisk)
url: https://arxiv.org/abs/2506.21575
date: 2025-06-15
venue: arXiv 2025
tags: [intent-grounding, data-query-agents, knowledge-graph, arxiv, semantic-layer-corpus]
---

# STRuCT-LLM: Unifying Tabular and Graph Reasoning with Reinforcement Learning for Semantic Parsing

**arXiv:** [2506.21575](https://arxiv.org/abs/2506.21575) · 2025-06-15 · arXiv 2025
**Authors:** Josefa Lia Stoisser et al. (Novo Nordisk)

> Abstract-tier note (extended-search corpus, not in the local agents-centric census). Part of the intent-grounding / semantic-layer thread (2026-06-23).

## Abstract
We propose STRuCT-LLM, a unified framework for training large language models (LLMs) to perform structured reasoning over both relational and graph-structured data. Our approach jointly optimizes Text-to-SQL and Text-to-Cypher tasks using reinforcement learning (RL) combined with Chain-of-Thought (CoT) supervision. To support fine-grained optimization in graph-based parsing, we introduce a topology-aware reward function based on graph edit distance. Unlike prior work that treats relational and graph formalisms in isolation, STRuCT-LLM leverages shared abstractions between SQL and Cypher to induce cross-formalism transfer, enabling SQL training to improve Cypher performance and vice versa - even without shared schemas. Our largest model (QwQ-32B) achieves substantial relative improvements across tasks: on semantic parsing, Spider improves by 13.5% and Text2Cypher by 73.1%. The model also demonstrates strong zero-shot generalization, improving performance on downstream tabular QA (TableBench: 8.5%) and knowledge graph QA (CR-LT-KGQA: 1.7%) without any QA-specific supervision. These results demonstrate both the effectiveness of executable queries as scaffolds for structured reasoning and the synergistic benefits of jointly training on SQL and Cypher.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[data-query-agents|Data-query agents]] · [[knowledge-graph|Knowledge graph]]
