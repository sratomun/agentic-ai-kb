---
type: source
source_type: arxiv
title: "Experience-Driven Multi-Agent Systems Are Training-free Context-aware Earth Observers"
authors: Pengyu Dai, Weihao Xuan, Junjue Wang, Hongruixuan Chen et al.
url: https://arxiv.org/abs/2602.02559v1
date: 2026-01-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agent-reliability, self-evolving-agents, agentic-rag, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Experience-Driven Multi-Agent Systems Are Training-free Context-aware Earth Observers

**arXiv:** [2602.02559v1](https://arxiv.org/abs/2602.02559v1) · 2026-01-30 · cs.AI
**Authors:** Pengyu Dai, Weihao Xuan, Junjue Wang, Hongruixuan Chen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances have enabled large language model (LLM) agents to solve complex tasks by orchestrating external tools. However, these agents often struggle in specialized, tool-intensive domains that demand long-horizon execution, tight coordination across modalities, and strict adherence to implicit tool constraints. Earth Observation (EO) tasks exemplify this challenge due to the multi-modal and multi-temporal data inputs, as well as the requirements of geo-knowledge constraints (spectrum library, spatial reasoning, etc): many high-level plans can be derailed by subtle execution errors that propagate through a pipeline and invalidate final results. A core difficulty is that existing agents lack a mechanism to learn fine-grained, tool-level expertise from interaction. Without such expertise, they cannot reliably configure tool parameters or recover from mid-execution failures, limiting their effectiveness in complex EO workflows. To address this, we introduce \textbf{GeoEvolver}, a self-evolving multi-agent system~(MAS) that enables LLM agents to acquire EO expertise through structured interaction without any parameter updates. GeoEvolver decomposes each query into independent sub-goals via a retrieval-augmented multi-agent orchestrator, then explores diverse tool-parameter configurations at the sub-goal level. Successful patterns and root-cause attribution from failures are then distilled in an evolving memory bank that provides in-context demonstrations for future queries. Experiments on three tool-integrated EO benchmarks show that GeoEvolver consistently improves end-to-end task success, with an average gain of 12\% across multiple LLM backbones, demonstrating that EO expertise can emerge progressively from efficient, fine-grained interactions with the environment.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.02559v1)
