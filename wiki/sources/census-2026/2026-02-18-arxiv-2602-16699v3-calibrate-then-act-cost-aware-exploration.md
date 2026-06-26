---
type: source
source_type: arxiv
title: "Calibrate-Then-Act: Cost-Aware Exploration in LLM Agents"
authors: Wenxuan Ding, Nicholas Tomlin, Greg Durrett
url: https://arxiv.org/abs/2602.16699v3
date: 2026-02-18
depth: abstract
auto: true
score: 6
primary: cs.CL
tags: [intent-understanding, human-agent-interaction, arxiv, auto-ingested]
---

# Calibrate-Then-Act: Cost-Aware Exploration in LLM Agents

**arXiv:** [2602.16699v3](https://arxiv.org/abs/2602.16699v3) · 2026-02-18 · cs.CL
**Authors:** Wenxuan Ding, Nicholas Tomlin, Greg Durrett

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived. Part of the intent-understanding corpus (2026-06-23).

## Abstract
LLM agents are deployed in environments where they must interact to acquire information. In these scenarios, the agent must reason about inherent cost-uncertainty tradeoffs in how to act, such as when to stop exploring and commit to an answer. For instance, on a programming task, an agent might run the code it generates, or it might generate tests for that code snippet; the cost of writing and running a test is nonzero, but typically lower than the cost of running buggy code. In this work, we show that we can induce LLM agents to explicitly reason about balancing these cost-uncertainty tradeoffs, then act more optimally in their environments. We formalize multiple tasks, including retrieval-augmented QA and a file reading coding task, as sequential decision-making problems under uncertainty. Each problem has latent environment state that impacts the agent's performance. We introduce a framework called Calibrate-Then-Act (CTA), where we pass the agent an inferred prior about this environment state to enable it to act more optimally. This information qualitatively changes agent behavior, and adds environment sensitivity to the agent which is not learned via standard RL training. Our results on a synthetic task, QA, and file reading show that making cost-benefit tradeoffs explicit with CTA helps agents discover more optimal decision-making strategies.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[human-agent-interaction|Human-agent interaction]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16699v3)
