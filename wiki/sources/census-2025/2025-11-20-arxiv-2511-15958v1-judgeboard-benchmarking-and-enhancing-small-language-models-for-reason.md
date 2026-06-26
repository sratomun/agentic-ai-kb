---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "JudgeBoard: Benchmarking and Enhancing Small Language Models for Reasoning Evaluation"
authors: Zhenyu Bi et al.
url: https://arxiv.org/abs/2511.15958v1
date: 2025-11-20
score: 13
primary: cs.AI
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, reasoning-models, multi-agent-systems, coding-agents]
---

# JudgeBoard: Benchmarking and Enhancing Small Language Models for Reasoning Evaluation

**arXiv:** [2511.15958v1](https://arxiv.org/abs/2511.15958v1) · 2025-11-20 · cs.AI
**Authors:** Zhenyu Bi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While small language models (SLMs) have shown promise on various reasoning tasks, their ability to judge the correctness of answers remains unclear compared to large language models (LLMs). Prior work on LLM-as-a-judge frameworks typically relies on comparing candidate answers against ground-truth labels or other candidate answers using predefined metrics like entailment. However, this approach is inherently indirect and difficult to fully automate, offering limited support for fine-grained and scalable evaluation of reasoning outputs. In this work, we propose JudgeBoard, a novel evaluation pipeline that directly queries models to assess the correctness of candidate answers without requiring extra answer comparisons. We focus on two core reasoning domains: mathematical reasoning and science/commonsense reasoning, and construct task-specific evaluation leaderboards using both accuracy-based ranking and an Elo-based rating system across five benchmark datasets, enabling consistent model comparison as judges rather than comparators. To improve judgment performance in lightweight models, we propose MAJ (Multi-Agent Judging), a novel multi-agent evaluation framework that leverages multiple interacting SLMs with distinct reasoning profiles to approximate LLM-level judgment accuracy through collaborative deliberation. Experimental results reveal a significant performance gap between SLMs and LLMs in isolated judging tasks. However, our MAJ framework substantially improves the reliability and consistency of SLMs. On the MATH dataset, MAJ using smaller-sized models as backbones performs comparatively well or even better than their larger-sized counterparts. Our findings highlight that multi-agent SLM systems can potentially match or exceed LLM performance in judgment tasks, with implications for scalable and efficient assessment.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[reasoning-models]] · [[multi-agent-systems]] · [[coding-agents]]
- **Census record:** `raw/arxiv/2025-census/census-2025.jsonl` (id 2511.15958v1)
