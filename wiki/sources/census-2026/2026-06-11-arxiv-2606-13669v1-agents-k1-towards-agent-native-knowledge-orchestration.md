---
type: source
source_type: arxiv
title: "Agents-K1: Towards Agent-native Knowledge Orchestration"
authors: Zongsheng Cao, Bihao Zhan, Jinxin Shi, Jiong Wang et al.
url: https://arxiv.org/abs/2606.13669v1
date: 2026-06-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [science-agents, knowledge-graph, agentic-rl, multi-agent-systems, arxiv, auto-ingested]
---

# Agents-K1: Towards Agent-native Knowledge Orchestration

**arXiv:** [2606.13669v1](https://arxiv.org/abs/2606.13669v1) · 2026-06-11 · cs.AI
**Authors:** Zongsheng Cao, Bihao Zhan, Jinxin Shi, Jiong Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Current LLM-based research agents have advanced through agent orchestration, yet largely overlook scientific knowledge orchestration. Existing works often reduce papers to abstracts, surface mentions, and flat \texttt{cites} edges, omitting key entities, claims, evidence, mechanisms, and method lineages essential for scientific reasoning. To this end, we introduce \textbf{Agents-K1}, an end-to-end knowledge orchestration pipeline that converts raw documents into agent-native scientific knowledge graphs. Agents-K1 integrates three components under a unifying theoretical foundation: a multimodal parser whose five-module schema captures entities, multimodal evidence, citations, and typed inter-entity relations across the full paper rather than abstracts alone; a 4B information-extraction backbone trained with GRPO under a rule-based reward; and a graphanything CLI, a tri-source agent interface that unifies web search, multimodal graph retrieval, and cross-document traversal. On top of this, we process 2.46 million scientific papers across six subjects to produce \textbf{Scholar-KG}, of which we release a one-million-paper subset, and the full Scholar-KG is accessible via the SCP link below. The same pipeline can be extended to general-domain corpora and to schema-conformant data synthesis. Extensive experiments demonstrate that Agents-K1 achieves superior performance in scientific information extraction, knowledge graph construction, and multi-hop scientific reasoning.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.13669v1)
