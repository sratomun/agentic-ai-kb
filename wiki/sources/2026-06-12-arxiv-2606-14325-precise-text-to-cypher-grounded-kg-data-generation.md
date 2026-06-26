---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Achieving Precise Text-To-Cypher Via Grounded Knowledge Graph Data Generation"
authors: Cazzaro, Lennon, Quattoni (Universitat Politècnica de Catalunya)
url: https://arxiv.org/abs/2606.14325
date: 2026-06-12
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, text-to-cypher, semantic-parsing, distillation, knowledge-graph]
---

# Achieving Precise Text-To-Cypher Via Grounded Knowledge Graph Data Generation

**arXiv [2606.14325](https://arxiv.org/abs/2606.14325)** · 2026-06-12 · UPC

**Significance.** The "tiny on-prem model rivals frontier" result for graph querying — graph-grounded synthetic data is the lever. Key currency node for [[text-to-cypher]] and ties to [[distillation]].

## Abstract
CYQUARK generates graph-grounded synthetic Text2Cypher data to fine-tune small, locally-deployable LLMs, with a flexible tree-pattern query generator and two filtering stages (semantic-constraint + LLM logical-meaning verification). Evaluated zero-shot via execution accuracy across 4 benchmarks / 19 graphs.

## From the paper (full-text, via subagent)
**Contribution / method.** **CYQUARK** extends prior SPOT with a tree-pattern generator covering multi-answer, nested, Union/Comparison/Subcall/Yes-No queries, regex, and aggregators, then filters generations by semantic constraints and an LLM logical-meaning verifier (80% recall / 66% precision on bad paraphrases; filtering adds ~6-9pp).
**Results.** Fine-tuning a **4B model on CYQUARK data lifts execution accuracy 37.94 → 76.21** (~2×); a **0.8B model reaches 73.30** — near **Claude Opus 4.7 (78.58)** and **GPT-5.5 (78.52)**. Zero-shot baselines: Qwen3.5-4B 37.94, 9B 41.21, 27B 60.67. On **CypherBench, CYQUARK-4B scores 85.38** avg.
**Takeaway.** Graph-grounded synthetic data buys data sovereignty: query a private knowledge graph with a tiny on-prem model instead of shipping it to a closed API, at near-frontier accuracy.

## Graph
- **Concepts:** [[text-to-cypher|Text-to-Cypher]] · [[semantic-parsing]] · [[distillation]] · [[knowledge-graph]]
- **Entities:** [[cypher]] · [[cypherbench]]
- **Raw:** full-text (alphaXiv, read via subagent) 2026-06-23
