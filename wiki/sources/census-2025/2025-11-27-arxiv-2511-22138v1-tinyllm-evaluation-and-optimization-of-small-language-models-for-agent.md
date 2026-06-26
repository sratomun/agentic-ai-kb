---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "TinyLLM: Evaluation and Optimization of Small Language Models for Agentic Tasks on Edge Devices"
authors: Mohd Ariful Haque et al.
url: https://arxiv.org/abs/2511.22138v1
date: 2025-11-27
score: 17
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge, post-training]
---

# TinyLLM: Evaluation and Optimization of Small Language Models for Agentic Tasks on Edge Devices

**arXiv:** [2511.22138v1](https://arxiv.org/abs/2511.22138v1) · 2025-11-27 · cs.LG
**Authors:** Mohd Ariful Haque et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This paper investigates the effectiveness of small language models (SLMs) for agentic tasks (function/tool/API calling) with a focus on running agents on edge devices without reliance on cloud infrastructure. We evaluate SLMs using the Berkeley Function Calling Leaderboard (BFCL) framework and describe parameter-driven optimization strategies that include supervised fine-tuning (SFT), parameter-efficient fine-tuning (PEFT), reinforcement learning (RL)-based optimization, preference alignment via Direct Preference Optimization (DPO), and hybrid methods. We report results for models including TinyAgent, TinyLlama, Qwen, and xLAM across BFCL categories (simple, multiple, parallel, parallel-multiple, and relevance detection), both in live and non-live settings, and in multi-turn evaluations. We additionally detail a DPO training pipeline constructed from AgentBank data (e.g., ALFRED), including our conversion of SFT data to chosen-rejected pairs using TinyLlama responses as rejected outputs and manual validation. Our results demonstrate clear accuracy differences across model scales where medium-sized models (1-3B parameters) significantly outperform ultra-compact models (<1B parameters), achieving up to 65.74% overall accuracy, and 55.62% multi-turn accuracy with hybrid optimization. This study highlights the importance of hybrid optimization strategies that enable small language models to deliver accurate, efficient, and stable agentic AI on edge devices, making privacy-preserving, low-latency autonomous agents practical beyond the cloud.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]] · [[post-training]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.22138v1)
