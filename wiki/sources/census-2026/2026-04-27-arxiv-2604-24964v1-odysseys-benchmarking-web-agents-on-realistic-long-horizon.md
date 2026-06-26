---
type: source
source_type: arxiv
title: "Odysseys: Benchmarking Web Agents on Realistic Long Horizon Tasks"
authors: Lawrence Keunho Jang, Jing Yu Koh, Daniel Fried, Ruslan Salakhutdinov
url: https://arxiv.org/abs/2604.24964v1
date: 2026-04-27
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [computer-use-agents, embodied-agents, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# Odysseys: Benchmarking Web Agents on Realistic Long Horizon Tasks

**arXiv:** [2604.24964v1](https://arxiv.org/abs/2604.24964v1) · 2026-04-27 · cs.LG
**Authors:** Lawrence Keunho Jang, Jing Yu Koh, Daniel Fried, Ruslan Salakhutdinov

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing web agent benchmarks have largely converged on short, single-site tasks that frontier models are approaching saturation on. However, real world web use consists of long-horizon, multi-site workflows. Common web navigation tasks, such as comparing products across different domains, planning trips across multiple services, or summarizing information from multiple search queries, require sustained context and cross-site reasoning over potentially hours of browsing. To capture and evaluate such behaviors, we introduce Odysseys: a benchmark of 200 long-horizon web tasks derived from real world browsing sessions evaluated on the live Internet. We find that binary pass/fail evaluation is inadequate for long-horizon settings and introduce a rubric-based evaluation, annotating each Odysseys task with an average of 6.1 graded rubrics. We demonstrate that this yields higher agreement with humans and provides a more fine-grained signal than commonly used trajectory-level LLM-as-a-judge evaluation metrics. We tested several leading frontier models and find that the strongest models achieve a success rate of 44.5%, which leaves substantial room for future improvements. Beyond task success, we argue that efficiency is a first-class concern for long-horizon agents. We introduce a Trajectory Efficiency metric (rubric score per step) and find that even frontier agents achieve only 1.15%, marking an evident need for agents that can succeed efficiently and not simply eventually. Odysseys isolates the critical evaluation of long-horizon proficiency in open-web environments, providing a realistic benchmark to measure progress towards computer-use agents that can potentially productively operate for hours. We release our tasks, evaluation scripts, and other results at https://odysseys-website.pages.dev

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.24964v1)
