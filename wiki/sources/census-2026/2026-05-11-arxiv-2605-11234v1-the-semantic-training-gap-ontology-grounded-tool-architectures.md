---
type: source
source_type: arxiv
title: "The Semantic Training Gap: Ontology-Grounded Tool Architectures for Industrial AI Agent Systems"
authors: Grama Chethan
url: https://arxiv.org/abs/2605.11234v1
date: 2026-05-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.AI
tags: [knowledge-graph, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# The Semantic Training Gap: Ontology-Grounded Tool Architectures for Industrial AI Agent Systems

**arXiv:** [2605.11234v1](https://arxiv.org/abs/2605.11234v1) · 2026-05-11 · cs.AI
**Authors:** Grama Chethan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM)-based AI agents are increasingly deployed in manufacturing environments for analytics, quality management, and decision support. These agents demonstrate statistical fluency with domain terminology but lack grounded understanding of operational semantics -- the relational structure that connects equipment identifiers, process parameters, failure codes, and regulatory constraints within a specific production context. This paper identifies and formalizes the semantic training gap: a structural disconnect between how AI systems acquire domain vocabulary through training and how manufacturing operations define meaning through ontological relationships. We demonstrate that this gap causes operationally incorrect outputs even when model responses are linguistically precise, and that in multi-agent configurations it produces a compounding failure mode we term semantic drift. To close this gap, we present an architecture that embeds manufacturing ontology directly into the AI tool layer as a typed relational configuration, enforcing semantic constraints at runtime rather than relying on model training. The architecture is formalized as a three-operation interface contract -- resolve, contextualize, annotate -- with invariants enforced by an AIOps orchestration layer. In a controlled experiment across six industry configurations (72 tool invocations using Qwen3-32B), unconstrained tool parameters produced a 43% hallucination rate for domain identifiers; ontology-grounded parameters reduced this to 0%. We validate the approach through a digital twin analytics platform demonstrating that a single codebase with domain-specific ontology configurations eliminates tool-call hallucination and achieves cross-domain configurability without application code changes.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.11234v1)
