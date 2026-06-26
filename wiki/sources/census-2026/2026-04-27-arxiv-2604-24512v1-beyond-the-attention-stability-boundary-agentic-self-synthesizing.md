---
type: source
source_type: arxiv
title: "Beyond the Attention Stability Boundary: Agentic Self-Synthesizing Reasoning Protocols"
authors: Dahlia Shehata, Ming Li
url: https://arxiv.org/abs/2604.24512v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [governance-gap, arxiv, auto-ingested]
---

# Beyond the Attention Stability Boundary: Agentic Self-Synthesizing Reasoning Protocols

**arXiv:** [2604.24512v1](https://arxiv.org/abs/2604.24512v1) · 2026-04-27 · cs.AI
**Authors:** Dahlia Shehata, Ming Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As LLM agents transition to autonomous digital coworkers, maintaining deterministic goal-directedness in non-linear multi-turn conversations emerged as an architectural bottleneck. We identify and formalize a systemic failure mode termed the Attention Latch in decoder-only autoregressive Transformers. This phenomenon, a behavioral manifestation of Information Over-squashing, occurs when the cumulative probabilistic weight of historical context overrides mid-task updates, causing agents to remain anchored to obsolete constraints despite explicit contradictory instructions. We propose Self-Synthesizing Reasoning Protocols (SSRP), a metacognitive framework that implements a discrete separation between high-level architectural planning (Architect) and turn-by-turn procedural execution (Executive). We evaluate SSRP across 9K trajectories using the MultiWOZ 2.2 dataset and the Aggregate Pivot Accuracy (APA), a novel metric we validate by mapping its scores to the U-shaped 'Lost in the Middle' curve. We present 3 experimental tiers: a shallow recency-based retrieval pilot, a high-entropy SOP, and a semantic hijacked 3-hop Multi-Fact Synthesis task. Our results empirically locate the Attention Stability Boundary, where stateless Vanilla ReAct baselines for GPT 5.4 collapse to 0.1% success while SSRP achieves a 715X Resilience Lift. We demonstrate statistically significant gains across Gemini 3.1 Pro, Claude Sonnet 4.6 and DeepSeek V3.2. Audits confirm SSRP necessity by proving attentional lapse via a recursive reflexion baseline (100% success); decoupling the latch from positional bias through equidistant stress testing (90% accuracy); and formalizing SSRP via the Information Bottleneck principle and granularity ablations. Procedural Integrity audit (98.8% adherence) reveals a Grounding Paradox where high-stability models fail by refusing to hallucinate under retrieval-reasoning contamination.

## Graph
- **Concepts:** [[governance-gap|Governance gap]]
- **Entities:** [[claude]] · [[gemini]] · [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.24512v1)
