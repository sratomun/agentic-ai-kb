---
type: source
source_type: arxiv
title: "Don't Retrieve, Navigate: Distilling Enterprise Knowledge into Navigable Agent Skills for QA and RAG"
authors: Yiqun Sun, Pengfei Wei, Lawrence B. Hsieh
url: https://arxiv.org/abs/2604.14572v3
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.IR
tags: [embodied-agents, agent-skills, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Don't Retrieve, Navigate: Distilling Enterprise Knowledge into Navigable Agent Skills for QA and RAG

**arXiv:** [2604.14572v3](https://arxiv.org/abs/2604.14572v3) · 2026-04-16 · cs.IR
**Authors:** Yiqun Sun, Pengfei Wei, Lawrence B. Hsieh

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Retrieval-Augmented Generation (RAG) grounds LLM responses in external evidence but treats the model as a passive consumer of search results, with no view of how the corpus is organized or what it has not yet seen. We present Corpus2Skill, which distills a document corpus offline into a hierarchical skill directory and lets an LLM agent navigate it at serve time, drilling from a bird's-eye view through progressively finer summaries down to documents, and backtracking when a branch is unproductive. On an enterprise customer-support benchmark, Corpus2Skill improves both answer quality and grounding over single-shot dense, hybrid, hierarchical-retrieval, and agentic RAG baselines at a moderate cost tradeoff. A ten-subset generalization study further shows that corpus navigation is not a universal replacement for retrieval: it consistently helps on single-domain corpora with a recoverable topical taxonomy, but flat retrieval remains preferable on open-domain factoid pools or homogeneous-tabular corpora that defeat top-level clustering. We characterize this scope distinction and discuss it as a design guideline for knowledge-grounded systems. Code is available at https://github.com/dukesun99/Corpus2Skill.

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-skills|Agent skills]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14572v3)
