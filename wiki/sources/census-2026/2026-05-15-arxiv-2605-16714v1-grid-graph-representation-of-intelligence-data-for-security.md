---
type: source
source_type: arxiv
title: "GRID: Graph Representation of Intelligence Data for Security Text Knowledge Graph Construction"
authors: Liangyi Huang, Zichen Liu, Fei Shao, Shang Ma et al.
url: https://arxiv.org/abs/2605.16714v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 3
primary: cs.AI
tags: [knowledge-graph, agentic-rl, agent-security, agent-memory, arxiv, auto-ingested]
---

# GRID: Graph Representation of Intelligence Data for Security Text Knowledge Graph Construction

**arXiv:** [2605.16714v1](https://arxiv.org/abs/2605.16714v1) · 2026-05-15 · cs.AI
**Authors:** Liangyi Huang, Zichen Liu, Fei Shao, Shang Ma et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Security knowledge graphs can provide computable external memory for security agents, but constructing them from long-form cyber threat intelligence (CTI) remains difficult: LLMs often lack grounded security-domain knowledge, and end-to-end document-to-graph training is hard to supervise with cheap, stable rewards. We present GRID (Graph Representation of Intelligence Data), an end-to-end framework for security text knowledge graph construction. GRID first builds security-domain supervision from CTI articles by creating traceable article-graph alignments through graph extraction and knowledge-graph-conditioned text revision. It then turns document-to-graph learning into a scripted task bank combining four-option multi-select questions with triple-level regex matching targets, yielding more stable task-specific rewards than repeatedly scoring full graph outputs with an LLM judge. Using this supervision pipeline, we train two Qwen3-4B-Instruct-2507-based 4B extractors: a primary Task-bank Reward model and a secondary End2End Reward model with LLM-as-judge precision/recall rewards. On 249 CTI articles from GRID, CASIE, CTINexus, MalKG, and SecureNLP, the Task-bank Reward model with the ontology-guided GRID extraction pipeline reaches 84.62% source-averaged precision, 64.91% source-averaged recall, and 68.53% Avg F1, achieving the best source-averaged recall and near-top Avg F1 with lower token usage and deployment cost. The End2End Reward model reaches 76.91% precision, 53.85% recall, and 58.06% Avg F1. Further analyses show that task-bank rewards can be built once offline and reused across later post-training runs, outperforming online End2End LLM-as-judge reward and weaker alternatives such as Choice-only Reward and End2End SFT without RL.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16714v1)
