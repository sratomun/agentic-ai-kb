---
type: source
source_type: arxiv
title: "Graph-Native Cognitive Memory for AI Agents: Formal Belief Revision Semantics for Versioned Memory Architectures"
authors: Young Bin Park
url: https://arxiv.org/abs/2603.17244v1
date: 2026-03-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.AI
tags: [knowledge-graph, agent-security, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Graph-Native Cognitive Memory for AI Agents: Formal Belief Revision Semantics for Versioned Memory Architectures

**arXiv:** [2603.17244v1](https://arxiv.org/abs/2603.17244v1) · 2026-03-18 · cs.AI
**Authors:** Young Bin Park

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While individual components for AI agent memory exist in prior systems, their architectural synthesis and formal grounding remain underexplored. We present Kumiho, a graph-native cognitive memory architecture grounded in formal belief revision semantics. The structural primitives required for cognitive memory -- immutable revisions, mutable tag pointers, typed dependency edges, URI-based addressing -- are identical to those required for managing agent-produced work as versionable assets, enabling a unified graph-native architecture that serves both purposes. The central formal contribution is a correspondence between the AGM belief revision framework and the operational semantics of a property graph memory system, proving satisfaction of the basic AGM postulates (K*2--K*6) and Hansson's belief base postulates (Relevance, Core-Retainment). The architecture implements a dual-store model (Redis working memory, Neo4j long-term graph) with hybrid fulltext and vector retrieval. On LoCoMo (token-level F1), Kumiho achieves 0.565 overall F1 (n=1,986) including 97.5% adversarial refusal accuracy. On LoCoMo-Plus, a Level-2 cognitive memory benchmark testing implicit constraint recall, Kumiho achieves 93.3% judge accuracy (n=401); independent reproduction by the benchmark authors yielded results in the mid-80% range, still substantially outperforming all published baselines (best: Gemini 2.5 Pro, 45.7%). Three architectural innovations drive the results: prospective indexing (LLM-generated future-scenario implications indexed at write time), event extraction (structured causal events preserved in summaries), and client-side LLM reranking. The architecture is model-decoupled: switching the answer model from GPT-4o-mini (~88%) to GPT-4o (93.3%) improves end-to-end accuracy without pipeline changes, at a total evaluation cost of ~$14 for 401 entries.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.17244v1)
