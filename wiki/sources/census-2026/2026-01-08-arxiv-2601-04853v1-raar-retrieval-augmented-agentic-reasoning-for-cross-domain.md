---
type: source
source_type: arxiv
title: "RAAR: Retrieval Augmented Agentic Reasoning for Cross-Domain Misinformation Detection"
authors: Zhiwei Liu, Runteng Guo, Baojie Qu, Yuechen Jiang et al.
url: https://arxiv.org/abs/2601.04853v1
date: 2026-01-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agentic-rl, agentic-rag, multi-agent-systems, arxiv, auto-ingested]
---

# RAAR: Retrieval Augmented Agentic Reasoning for Cross-Domain Misinformation Detection

**arXiv:** [2601.04853v1](https://arxiv.org/abs/2601.04853v1) · 2026-01-08 · cs.CL
**Authors:** Zhiwei Liu, Runteng Guo, Baojie Qu, Yuechen Jiang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Cross-domain misinformation detection is challenging, as misinformation arises across domains with substantial differences in knowledge and discourse. Existing methods often rely on single-perspective cues and struggle to generalize to challenging or underrepresented domains, while reasoning large language models (LLMs), though effective on complex tasks, are limited to same-distribution data. To address these gaps, we introduce RAAR, the first retrieval-augmented agentic reasoning framework for cross-domain misinformation detection. To enable cross-domain transfer beyond same-distribution assumptions, RAAR retrieves multi-perspective source-domain evidence aligned with each target sample's semantics, sentiment, and writing style. To overcome single-perspective modeling and missing systematic reasoning, RAAR constructs verifiable multi-step reasoning paths through specialized multi-agent collaboration, where perspective-specific agents produce complementary analyses and a summary agent integrates them under verifier guidance. RAAR further applies supervised fine-tuning and reinforcement learning to train a single multi-task verifier to enhance verification and reasoning capabilities. Based on RAAR, we trained the RAAR-8b and RAAR-14b models. Evaluation on three cross-domain misinformation detection tasks shows that RAAR substantially enhances the capabilities of the base models and outperforms other cross-domain methods, advanced LLMs, and LLM-based adaptation approaches. The project will be released at https://github.com/lzw108/RAAR.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-rag|Agentic RAG]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.04853v1)
