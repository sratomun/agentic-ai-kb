---
type: source
source_type: arxiv
title: "Extracting Semantics: LLM-Guided Automatic Population of Robot Ontology from URDF"
authors: Bastien Dussard, Guillaume Sarthou
url: https://arxiv.org/abs/2606.17073v1
date: 2026-06-10
ingested: 2026-06-21
depth: abstract
auto: true
score: 2
primary: cs.RO
tags: [embodied-agents, knowledge-graph, agent-reliability, arxiv, auto-ingested]
---

# Extracting Semantics: LLM-Guided Automatic Population of Robot Ontology from URDF

**arXiv:** [2606.17073v1](https://arxiv.org/abs/2606.17073v1) · 2026-06-10 · cs.RO
**Authors:** Bastien Dussard, Guillaume Sarthou

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While commonsense knowledge may suffice for virtual agents, embodied robots interacting with humans require grounded and semantically rich representations of both their environment and their own physical embodiment. In cognitive robotics, ontologies are effective for integrating such heterogeneous knowledge to enable explainable reasoning, even during continuous knowledge updates. Yet, their manual construction remains a bottleneck. We present a preliminary approach for the automatic generation of robot semantic abstractions by transforming Unified Robot Description Format (URDF) models into populated ontologies. Although URDF files provide structural and kinematic descriptions, their identifiers often require commonsense interpretation to recover meaningful semantics, a task at which Large Language Models (LLMs) excel. Our pipeline leverages LLMs to infer semantic relationships by prompting them with concepts from an existing ontology, ensuring the final classification remains aligned with the formal model. To improve reliability, the pipeline combines majority voting across multiple LLM queries along with syntactic and schema-level validation to ensure that generated outputs conform to the expected representation format and ontology constraints. We evaluate the approach on multiple robot descriptions and discuss the generated abstractions. Initial results indicate that the proposed method can effectively bridge the gap between low-level robot descriptions and the structured, grounded knowledge representations required for human-robot interaction.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.17073v1)
