---
type: source
source_type: arxiv
title: "Helicase: Uncertainty-Guided Supply Chain Knowledge Graph Construction with Autonomous Multi-Agent LLMs"
authors: Yunbo Long, Haolang Zhao, Ge Zheng, Alexandra Brintrup
url: https://arxiv.org/abs/2605.26835v1
date: 2026-05-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.AI
tags: [coding-agents, knowledge-graph, agent-reliability, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Helicase: Uncertainty-Guided Supply Chain Knowledge Graph Construction with Autonomous Multi-Agent LLMs

**arXiv:** [2605.26835v1](https://arxiv.org/abs/2605.26835v1) · 2026-05-26 · cs.AI
**Authors:** Yunbo Long, Haolang Zhao, Ge Zheng, Alexandra Brintrup

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based multi-agent systems have been widely adopted for knowledge retrieval and report generation, synthesizing known information through web search and textual reasoning. However, many critical information tasks in supply chains are not simple one-shot queries: they are structural inference problems requiring multi-hop reasoning across complex, fragmented web resources. Questions such as \textit{``Which Tesla components use lithium from Australian mines?''} have no answer in any single document; answers must be computationally synthesized through the autonomous construction and analysis of dynamic knowledge graphs assembled from fragmented, heterogeneous sources. Moreover, such discovery processes must be uncertainty-aware: decisions depend not only on answers but on calibrated confidence in their reliability, traceable to source quality and reasoning consistency. To address this capability gap, we propose \textit{Helicase}, an autonomous multi-agent LLM system for uncertainty-guided supply chain knowledge graph construction. \textit{Helicase} decomposes high-level supply-chain queries into executable investigation plans, coordinates specialized web-search, reasoning, and coding agents through iterative verification loops, and incrementally constructs query-specific supply chain knowledge graphs with per-fact uncertainty annotations. Its three-layer uncertainty framework tracks uncertainty at the action, trajectory, and memory layers, enabling both structural inference and calibrated confidence assessment. To evaluate autonomous reasoning across the full complexity spectrum, we introduce SCQA (Supply Chain Query Assessment), a benchmark of 80 supply chain queries organized into four quadrants spanning single-hop to multi-hop inference under both high and low data visibility.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26835v1)
