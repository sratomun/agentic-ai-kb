---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Fathom-DeepResearch: Unlocking Long Horizon Information Retrieval and Synthesis for SLMs"
authors: Shreyas Singh et al.
url: https://arxiv.org/abs/2509.24107v1
date: 2025-09-28
score: 16
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, post-training, reasoning-models]
---

# Fathom-DeepResearch: Unlocking Long Horizon Information Retrieval and Synthesis for SLMs

**arXiv:** [2509.24107v1](https://arxiv.org/abs/2509.24107v1) · 2025-09-28 · cs.AI
**Authors:** Shreyas Singh et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Tool-integrated reasoning has emerged as a key focus for enabling agentic applications. Among these, DeepResearch Agents have gained significant attention for their strong performance on complex, open-ended information-seeking tasks. We introduce Fathom-DeepResearch, an agentic system composed of two specialized models. The first is Fathom-Search-4B, a DeepSearch model trained from Qwen3-4B and optimized for evidence-based investigation through live web search and targeted webpage querying. Its training combines three advances: (i) DUETQA, a 5K-sample dataset generated via multi-agent self-play that enforces strict web-search dependence and heterogeneous source grounding; (ii) RAPO, a zero-overhead extension of GRPO that stabilizes multi-turn Reinforcement Learning with Verifiable Rewards through curriculum pruning, reward-aware advantage scaling, and per-prompt replay buffers; and (iii) a steerable step-level reward that classifies each tool call by cognitive behavior and marginal utility, enabling explicit control over search trajectory breadth, depth, and horizon. These improvements enable reliable extension of tool-calling beyond 20 calls when warranted. The second is Fathom-Synthesizer-4B, trained from Qwen3-4B, which converts multi-turn DeepSearch traces into structured, citation-dense DeepResearch Reports for comprehensive synthesis. Evaluated on DeepSearch benchmarks (SimpleQA, FRAMES, WebWalker, Seal0, MuSiQue) and DeepResearch-Bench, the system achieves state-of-the-art performance in the open-weights category while demonstrating strong generalization to diverse reasoning tasks including HLE, AIME-25, GPQA-Diamond, and MedQA.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2509.24107v1)
