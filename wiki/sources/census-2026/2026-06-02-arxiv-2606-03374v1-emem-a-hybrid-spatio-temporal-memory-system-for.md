---
type: source
source_type: arxiv
title: "eMEM: A Hybrid Spatio-Temporal Memory System For Embodied Agents"
authors: A. Haroon Rasheed, Maria Kabtoul
url: https://arxiv.org/abs/2606.03374v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.RO
tags: [clinical-agents, embodied-agents, knowledge-graph, agentic-rag, agent-memory, arxiv, auto-ingested]
---

# eMEM: A Hybrid Spatio-Temporal Memory System For Embodied Agents

**arXiv:** [2606.03374v1](https://arxiv.org/abs/2606.03374v1) · 2026-06-02 · cs.RO
**Authors:** A. Haroon Rasheed, Maria Kabtoul

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present eMEM (Embodied Memory), a hybrid graph-based memory system for embodied agents operating in physical environments. Current agent memory architectures, such as Generative Agents, MemGPT, and A-MEM, treat memory as text streams or knowledge graphs, but embodied agents require memory that is simultaneously searchable by meaning, space, and time. eMEM fills this gap with a multi-index architecture (SQL ITE for structured storage, hnswlib for approximate nearest neighbour semantic search, and an R-tree for spatial queries) unified behind a single graph model. A tiered consolidation pipeline transforms raw perceptual observations into compressed summaries, mirroring hippocampal-neocortical consolidation in biological systems. Ten agent-facing recall tools expose memory retrieval primitives, including concept-to-location resolution and cross layer recall, as first-class operations for LLM tool calling. The system is fully embedded and runs in-process alongside the agent. In addition we introduce eMEM-Bench v1, a benchmark we construct over ProcTHOR-10K scenes for embodied memory evaluation. The benchmark is organised explicitly around eight cognitive-psychology paradigms (DRM lures, pattern separation, pattern completion, source monitoring, context-dependent retrieval, long-horizon interference, serial position, and a foil augmented retention curve), each chosen so that the result is interpretable against the broader memory-systems literature in humans and prior agent-memory systems; a level of diagnostic that surface-task benchmarks like LoCoMo or OpenEQA cannot provide. eMEM scores 80.8 weighted mean over 988 probes, with a flat retention curve at ceiling from 1 h to 1 yr of simulated delay on room-unique items. We show that a pure RAG baseline (the flat_rag ablation) loses 30 pt on context dependent retrieval and 29 pt on DRM lure rejection, isolating the contribution of multi-layer storage and consolidation respectively. We release both the system and the benchmark code.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03374v1)
