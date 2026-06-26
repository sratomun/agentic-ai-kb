---
type: source
source_type: arxiv
title: "Insight Agents: An LLM-Based Multi-Agent System for Data Insights"
authors: Jincheng Bai, Zhenyu Zhang, Jennifer Zhang, Zhihuai Zhu
url: https://arxiv.org/abs/2601.20048v2
date: 2026-01-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [science-agents, multi-agent-systems, arxiv, auto-ingested]
---

# Insight Agents: An LLM-Based Multi-Agent System for Data Insights

**arXiv:** [2601.20048v2](https://arxiv.org/abs/2601.20048v2) · 2026-01-27 · cs.AI
**Authors:** Jincheng Bai, Zhenyu Zhang, Jennifer Zhang, Zhihuai Zhu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Today, E-commerce sellers face several key challenges, including difficulties in discovering and effectively utilizing available programs and tools, and struggling to understand and utilize rich data from various tools. We therefore aim to develop Insight Agents (IA), a conversational multi-agent Data Insight system, to provide E-commerce sellers with personalized data and business insights through automated information retrieval. Our hypothesis is that IA will serve as a force multiplier for sellers, thereby driving incremental seller adoption by reducing the effort required and increase speed at which sellers make good business decisions. In this paper, we introduce this novel LLM-backed end-to-end agentic system built on a plan-and-execute paradigm and designed for comprehensive coverage, high accuracy, and low latency. It features a hierarchical multi-agent structure, consisting of manager agent and two worker agents: data presentation and insight generation, for efficient information retrieval and problem-solving. We design a simple yet effective ML solution for manager agent that combines Out-of-Domain (OOD) detection using a lightweight encoder-decoder model and agent routing through a BERT-based classifier, optimizing both accuracy and latency. Within the two worker agents, a strategic planning is designed for API-based data model that breaks down queries into granular components to generate more accurate responses, and domain knowledge is dynamically injected to to enhance the insight generator. IA has been launched for Amazon sellers in US, which has achieved high accuracy of 90% based on human evaluation, with latency of P90 below 15s.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.20048v2)
