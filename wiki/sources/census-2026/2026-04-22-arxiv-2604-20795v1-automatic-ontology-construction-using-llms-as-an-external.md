---
type: source
source_type: arxiv
title: "Automatic Ontology Construction Using LLMs as an External Layer of Memory, Verification, and Planning for Hybrid Intelligent Systems"
authors: Pavel Salovskii, Iuliia Gorshkova
url: https://arxiv.org/abs/2604.20795v1
date: 2026-04-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [embodied-agents, knowledge-graph, agent-reliability, agentic-rag, agent-memory, arxiv, auto-ingested]
---

# Automatic Ontology Construction Using LLMs as an External Layer of Memory, Verification, and Planning for Hybrid Intelligent Systems

**arXiv:** [2604.20795v1](https://arxiv.org/abs/2604.20795v1) · 2026-04-22 · cs.AI
**Authors:** Pavel Salovskii, Iuliia Gorshkova

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper presents a hybrid architecture for intelligent systems in which large language models (LLMs) are extended with an external ontological memory layer. Instead of relying solely on parametric knowledge and vector-based retrieval (RAG), the proposed approach constructs and maintains a structured knowledge graph using RDF/OWL representations, enabling persistent, verifiable, and semantically grounded reasoning. The core contribution is an automated pipeline for ontology construction from heterogeneous data sources, including documents, APIs, and dialogue logs. The system performs entity recognition, relation extraction, normalization, and triple generation, followed by validation using SHACL and OWL constraints, and continuous graph updates. During inference, LLMs operate over a combined context that integrates vector-based retrieval with graph-based reasoning and external tool interaction. Experimental observations on planning tasks, including the Tower of Hanoi benchmark, indicate that ontology augmentation improves performance in multi-step reasoning scenarios compared to baseline LLM systems. In addition, the ontology layer enables formal validation of generated outputs, transforming the system into a generation-verification-correction pipeline. The proposed architecture addresses key limitations of current LLM-based systems, including lack of long-term memory, weak structural understanding, and limited reasoning capabilities. It provides a foundation for building agent-based systems, robotics applications, and enterprise AI solutions that require persistent knowledge, explainability, and reliable decision-making.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.20795v1)
