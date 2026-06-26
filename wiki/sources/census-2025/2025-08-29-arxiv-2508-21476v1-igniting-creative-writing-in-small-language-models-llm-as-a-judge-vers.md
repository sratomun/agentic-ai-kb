---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Igniting Creative Writing in Small Language Models: LLM-as-a-Judge versus Multi-Agent Refined Rewards"
authors: Xiaolong Wei et al.
url: https://arxiv.org/abs/2508.21476v1
date: 2025-08-29
score: 11
primary: cs.CL
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, multi-agent-systems]
---

# Igniting Creative Writing in Small Language Models: LLM-as-a-Judge versus Multi-Agent Refined Rewards

**arXiv:** [2508.21476v1](https://arxiv.org/abs/2508.21476v1) · 2025-08-29 · cs.CL
**Authors:** Xiaolong Wei et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have demonstrated remarkable creative writing capabilities, yet their substantial computational demands hinder widespread use. Enhancing Small Language Models (SLMs) offers a promising alternative, but current methods like Supervised Fine-Tuning (SFT) struggle with novelty, and Reinforcement Learning from Human Feedback (RLHF) is costly. This paper explores two distinct AI-driven reward strategies within a Reinforcement Learning from AI Feedback (RLAIF) framework to ignite the creative writing of a 7B-parameter SLM, specifically for generating Chinese greetings. The first strategy employs a RM trained on high-quality preference data curated by a novel multi-agent rejection sampling framework designed for creative tasks. The second, more novel strategy utilizes a principle-guided LLM-as-a-Judge, whose reward function is optimized via an adversarial training scheme with a reflection mechanism, to directly provide reward signals. Comprehensive experiments reveal that while both approaches significantly enhance creative output over baselines, the principle-guided LLM-as-a-Judge demonstrably yields superior generation quality. Furthermore, it offers notable advantages in training efficiency and reduced dependency on human-annotated data, presenting a more scalable and effective path towards creative SLMs. Our automated evaluation methods also exhibit strong alignment with human judgments. Our code and data are publicly available at https://github.com/weixiaolong94-hub/Igniting-Creative-Writing-in-Small-Language-Models.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[multi-agent-systems]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2508.21476v1)
