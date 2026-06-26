---
type: source
source_type: arxiv
title: "GraphWalk: Enabling Reasoning in Large Language Models through Tool-Based Graph Navigation"
authors: Taraneh Ghandi, Hamidreza Mahyar, Shachar Klaiman
url: https://arxiv.org/abs/2604.01610v1
date: 2026-04-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [embodied-agents, knowledge-graph, agentic-rag, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# GraphWalk: Enabling Reasoning in Large Language Models through Tool-Based Graph Navigation

**arXiv:** [2604.01610v1](https://arxiv.org/abs/2604.01610v1) · 2026-04-02 · cs.AI
**Authors:** Taraneh Ghandi, Hamidreza Mahyar, Shachar Klaiman

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The use of knowledge graphs for grounding agents in real-world Q&A applications has become increasingly common. Answering complex queries often requires multi-hop reasoning and the ability to navigate vast relational structures. Standard approaches rely on prompting techniques that steer large language models to reason over raw graph context, or retrieval-augmented generation pipelines where relevant subgraphs are injected into the context. These, however, face severe limitations with enterprise-scale KGs that cannot fit in even the largest context windows available today. We present GraphWalk, a problem-agnostic, training-free, tool-based framework that allows off-the-shelf LLMs to reason through sequential graph navigation, dramatically increasing performance across different tasks. Unlike task-specific agent frameworks that encode domain knowledge into specialized tools, GraphWalk equips the LLM with a minimal set of orthogonal graph operations sufficient to traverse any graph structure. We evaluate whether models equipped with GraphWalk can compose these operations into correct multi-step reasoning chains, where each tool call represents a verifiable step creating a transparent execution trace. We first demonstrate our approach on maze traversal, a problem non-reasoning models are completely unable to solve, then present results on graphs resembling real-world enterprise knowledge graphs. To isolate structural reasoning from world knowledge, we evaluate on entirely synthetic graphs with random, non-semantic labels. Our benchmark spans 12 query templates from basic retrieval to compound first-order logic queries. Results show that tool-based traversal yields substantial and consistent gains over in-context baselines across all model families tested, with gains becoming more pronounced as scale increases, precisely where in-context approaches fail catastrophically.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.01610v1)
