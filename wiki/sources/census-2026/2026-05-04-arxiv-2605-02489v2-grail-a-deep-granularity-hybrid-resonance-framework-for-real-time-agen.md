---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "GRAIL: A Deep-Granularity Hybrid Resonance Framework for Real-Time Agent Discovery via SLM-Enhanced Indexing"
authors: Jinliang Xu
url: https://arxiv.org/abs/2605.02489v2
date: 2026-05-04
score: 7
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, post-training, agentic-rag, multi-agent-systems, intent-routing]
---

# GRAIL: A Deep-Granularity Hybrid Resonance Framework for Real-Time Agent Discovery via SLM-Enhanced Indexing

**arXiv:** [2605.02489v2](https://arxiv.org/abs/2605.02489v2) · 2026-05-04 · cs.AI
**Authors:** Jinliang Xu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As the ecosystem of Large Language Model (LLM)-based agents expands rapidly, efficient and accurate Agent Discovery becomes a critical bottleneck for large-scale multi-agent collaboration. Existing approaches typically face a dichotomy: either relying on heavy-weight LLMs for intent parsing, leading to prohibitive latency (often exceeding 30 seconds), or using monolithic vector retrieval that sacrifices semantic precision for speed. To bridge this gap, we propose \textbf{GRAIL} (Granular Resonance-based Agent/AI Link), a novel framework achieving sub-400ms discovery latency without compromising accuracy. GRAIL introduces three key innovations: (1) \textbf{SLM-Enhanced Prediction}, replacing the generalized LLM parser with a specialized, fine-tuned Small Language Model (SLM) for millisecond-level capability tag prediction; (2) \textbf{Pseudo-Document Expansion}, augmenting agent descriptions with synthetic queries to enhance semantic density for robust dense retrieval; and (3) \textbf{MaxSim Resonance}, a fine-grained matching mechanism computing maximum similarity between user queries and discrete agent usage examples, effectively mitigating semantic dilution. Validated on \textbf{AgentTaxo-9K}, our new large-scale dataset of 9,240 agents, GRAIL reduces end-to-end discovery latency by over \textbf{79$\times$} compared to LLM-parsing baselines, while significantly outperforming traditional vector search in Recall@10. This framework offers a scalable, industrial-grade solution for the real-time ``Internet of Agents."

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[post-training]] · [[agentic-rag]] · [[multi-agent-systems]] · [[intent-routing]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.02489v2)
