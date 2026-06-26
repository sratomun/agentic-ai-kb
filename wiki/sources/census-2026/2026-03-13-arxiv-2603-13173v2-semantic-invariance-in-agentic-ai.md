---
type: source
source_type: arxiv
title: "Semantic Invariance in Agentic AI"
authors: I. de Zarzà, J. de Curtò, Jordi Cabot, Pietro Manzoni et al.
url: https://arxiv.org/abs/2603.13173v2
date: 2026-03-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Semantic Invariance in Agentic AI

**arXiv:** [2603.13173v2](https://arxiv.org/abs/2603.13173v2) · 2026-03-13 · cs.AI
**Authors:** I. de Zarzà, J. de Curtò, Jordi Cabot, Pietro Manzoni et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) increasingly serve as autonomous reasoning agents in decision support, scientific problem-solving, and multi-agent coordination systems. However, deploying LLM agents in consequential applications requires assurance that their reasoning remains stable under semantically equivalent input variations, a property we term semantic invariance. Standard benchmark evaluations, which assess accuracy on fixed, canonical problem formulations, fail to capture this critical reliability dimension. To address this shortcoming, in this paper we present a metamorphic testing framework for systematically assessing the robustness of LLM reasoning agents, applying eight semantic-preserving transformations (identity, paraphrase, fact reordering, expansion, contraction, academic context, business context, and contrastive formulation) across seven foundation models spanning four distinct architectural families: Hermes (70B, 405B), Qwen3 (30B-A3B, 235B-A22B), DeepSeek-R1, and gpt-oss (20B, 120B). Our evaluation encompasses 19 multi-step reasoning problems across eight scientific domains. The results reveal that model scale does not predict robustness: the smaller Qwen3-30B-A3B achieves the highest stability (79.6% invariant responses, semantic similarity 0.91), while larger models exhibit greater fragility.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[deepseek]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.13173v2)
