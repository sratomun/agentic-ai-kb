---
type: source
source_type: arxiv
title: "Memory is Reconstructed, Not Retrieved: Graph Memory for LLM Agents"
authors: Shuo Ji, Yibo Li, Bryan Hooi
url: https://arxiv.org/abs/2606.06036v1
date: 2026-06-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [knowledge-graph, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Memory is Reconstructed, Not Retrieved: Graph Memory for LLM Agents

**arXiv:** [2606.06036v1](https://arxiv.org/abs/2606.06036v1) · 2026-06-04 · cs.AI
**Authors:** Shuo Ji, Yibo Li, Bryan Hooi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Despite recent progress, LLM agents still struggle with reasoning over long interaction histories. While current memory-augmented agents rely on a static retrieve-then-reason paradigm, this rigid pipeline design prevents them from dynamically adapting memory access to intermediate evidence discovered during inference. To bridge this gap, we propose MRAgent, a framework that combines an associative memory graph with an active reconstruction mechanism. We represent memory as a Cue-Tag-Content graph, where associative tags serve as semantic bridges connecting fine-grained cues to memory contents. Operating on this structure, our active reconstruction mechanism integrates LLM reasoning directly into memory access, allowing the agent to iteratively explore and prune retrieval paths based on accumulated evidence. This ensures that memory retrieval is dynamically adapted to the reasoning context while avoiding combinatorial explosion caused by unconstrained expansion. Experiments on the LoCoMo benchmark and LongMemEval benchmark demonstrate significant improvements over strong baselines (up to 23%), while substantially reducing token and runtime cost, highlighting the effectiveness of active and associative reconstruction for long-horizon memory reasoning.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.06036v1)
