---
type: source
source_type: arxiv
title: "Exploring Reasoning Reward Model for Agents"
authors: Kaixuan Fan, Kaituo Feng, Manyuan Zhang, Tianshuo Peng et al.
url: https://arxiv.org/abs/2601.22154v2
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agentic-rl, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Exploring Reasoning Reward Model for Agents

**arXiv:** [2601.22154v2](https://arxiv.org/abs/2601.22154v2) · 2026-01-29 · cs.AI
**Authors:** Kaixuan Fan, Kaituo Feng, Manyuan Zhang, Tianshuo Peng et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Reinforcement Learning (Agentic RL) has achieved notable success in enabling agents to perform complex reasoning and tool use. However, most methods still relies on sparse outcome-based reward for training. Such feedback fails to differentiate intermediate reasoning quality, leading to suboptimal training results. In this paper, we introduce Agent Reasoning Reward Model (Agent-RRM), a multi-faceted reward model that produces structured feedback for agentic trajectories, including (1) an explicit reasoning trace , (2) a focused critique that provides refinement guidance by highlighting reasoning flaws, and (3) an overall score that evaluates process performance. Leveraging these signals, we systematically investigate three integration strategies: Reagent-C (text-augmented refinement), Reagent-R (reward-augmented guidance), and Reagent-U (unified feedback integration). Extensive evaluations across 12 diverse benchmarks demonstrate that Reagent-U yields substantial performance leaps, achieving 43.7% on GAIA and 46.2% on WebWalkerQA, validating the effectiveness of our reasoning reward model and training schemes. Code, models, and datasets are all released to facilitate future research.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gaia-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.22154v2)
