---
type: source
source_type: arxiv
title: "Learning to Present: Inverse Specification Rewards for Agentic Slide Generation"
authors: Karthik Ragunath Ananda Kumar, Subrahmanyam Arunachalam
url: https://arxiv.org/abs/2603.16839v1
date: 2026-03-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, tool-use, governance-gap, arxiv, auto-ingested]
---

# Learning to Present: Inverse Specification Rewards for Agentic Slide Generation

**arXiv:** [2603.16839v1](https://arxiv.org/abs/2603.16839v1) · 2026-03-17 · cs.AI
**Authors:** Karthik Ragunath Ananda Kumar, Subrahmanyam Arunachalam

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Automated presentation generation remains a challenging task requiring coherent content creation, visual design, and audience-aware communication. This work proposes an OpenEnv-compatible reinforcement learning environment where LLM agents learn to research topics, plan content, and generate professional HTML slide presentations through tool use. We introduce a multi-component reward system combining structural validation, render quality assessment, LLM-based aesthetic scoring, content quality metrics, and an inverse specification reward that measures how faithfully generated slides convey their intended purpose. The inverse specification reward, an "inverse task" where an LLM attempts to recover the original specification from generated slides, provides a holistic quality signal. Our approach fine-tunes Qwen2.5-Coder-7B via GRPO, training only 0.5% of parameters on prompts derived from expert demonstrations collected using Claude Opus 4.6. Experiments on 48 diverse business briefs across six models demonstrate that our fine-tuned 7B model achieves 91.2% of Claude Opus 4.6's quality while improving 33.1% over the base model. The six-model comparison reveals that instruction adherence and tool-use compliance, rather than raw parameter count, determine agentic task performance. We contribute SlideRL, an open-source dataset of 288 multi-turn rollout trajectories across all six models: https://huggingface.co/datasets/KarthikRagunathAnandaKumar/sliderl-multi-turn-rollouts Code: https://github.com/pushing-the-frontier/slide-forge-llm

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[governance-gap|Governance gap]]
- **Entities:** [[claude]] · [[qwen]] · [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.16839v1)
