---
type: source
source_type: arxiv
title: "GAAMA: Graph Augmented Associative Memory for Agents"
authors: Swarna Kamal Paul, Shubhendu Sharma, Nitin Sareen
url: https://arxiv.org/abs/2603.27910v2
date: 2026-03-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agentic-rl, agentic-rag, agent-memory, arxiv, auto-ingested]
---

# GAAMA: Graph Augmented Associative Memory for Agents

**arXiv:** [2603.27910v2](https://arxiv.org/abs/2603.27910v2) · 2026-03-29 · cs.AI
**Authors:** Swarna Kamal Paul, Shubhendu Sharma, Nitin Sareen

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents that interact with users across multiple sessions require persistent long-term memory to maintain coherent, personalized behavior. Current approaches either rely on flat retrieval-augmented generation (RAG), which loses structural relationships among memories, or use entity-centric knowledge graphs that suffer from mega-hub effects in conversational data, diluting graph-based relevance propagation. We propose GAAMA, a graph-augmented associative memory for agents that constructs a concept-mediated knowledge graph through a three-step pipeline: (1)verbatim episode preservation, (2)LLM-based extraction of atomic facts and topic-level concept nodes, and (3)synthesis of higher-order reflections. The resulting graph uses four node types (episode, fact, reflection, concept) connected by five structural edge types, with concept nodes providing cross-cutting traversal paths that avoid the mega-hub problem of entity-centric designs. Retrieval combines cosine-similarity-based k-nearest neighbor search with edge-type-aware Personalized PageRank (PPR) through an additive scoring function. We further introduce GRAFT (Graph Repair by Augmenting Facts & Topology), a post-retrieval corrective layer that diagnoses retrieval failures and surgically repairs the knowledge graph. On LoCoMo-10 (1,540 questions, 10 multi-session conversations), GAAMA achieves 79.1% mean reward, a +4.2~pp improvement over a tuned RAG baseline, the strongest comparator. On MemoryArena, GAAMA outperforms full-context baselines across three tasks - Group Travel (+0.4~pp), Web Shopping (+3.4~pp), and Progressive Search (+0.7~pp) - with advantages growing monotonically with dialogue length. Notably, GAAMA delivers consistent performance across all categories, matching the best competing method in each, whereas every competitor degrades in at least one category.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.27910v2)
