---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "PACE: Two-Timescale Self-Evolution for Small Language Model Agents"
authors: Chen Ling et al.
url: https://arxiv.org/abs/2605.23019v1
date: 2026-05-21
score: 9
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, tool-use, llm-as-judge]
---

# PACE: Two-Timescale Self-Evolution for Small Language Model Agents

**arXiv:** [2605.23019v1](https://arxiv.org/abs/2605.23019v1) · 2026-05-21 · cs.LG
**Authors:** Chen Ling et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Deploying language-model agents in production often requires substantial compute and human effort to tune prompts, parsers, validators, and other components of the agent pipeline. Self-evolution offers a promising alternative, but most existing frameworks assume access to frontier models that can reliably diagnose failures, propose revisions, and judge their own updates. We study whether frozen small language models (SLMs) can serve as effective self-evolving agents under resource constraints. We propose PACE (Prompt And Control Logic Evolution), a two-timescale framework that coordinates low-risk prompt refinement with higher-risk control-logic updates. PACE evolves prompts under fixed control logic until prompt-level gains saturate, then considers constrained control-logic updates that are accepted through held-out validation. Across three frozen SLM backbones ranging from 4B to 14B parameters and four controlled benchmarks, PACE achieves the best performance on all 12 backbone--benchmark combinations, improving over vanilla SLM agents by up to +9.2% relative improvement and over the stronger single-mode evolution baseline by up to +5.4% relative improvement. A tau-bench case study further shows that PACE improves multi-turn tool-use success over vanilla and prompt-only evolution. These results suggest that reliable SLM agent self-evolution is possible without updating model weights or relying on frontier-model teachers, and that the key benefit is not any single final solver pattern but autonomous, validated discovery of task-appropriate inference strategies.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[llm-as-judge]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23019v1)
