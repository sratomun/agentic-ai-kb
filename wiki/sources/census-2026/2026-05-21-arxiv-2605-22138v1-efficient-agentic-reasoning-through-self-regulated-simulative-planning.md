---
type: source
source_type: arxiv
title: "Efficient Agentic Reasoning Through Self-Regulated Simulative Planning"
authors: Mingkai Deng, Jinyu Hou, Lara Sá Neves, Varad Pimpalkhute et al.
url: https://arxiv.org/abs/2605.22138v1
date: 2026-05-21
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# Efficient Agentic Reasoning Through Self-Regulated Simulative Planning

**arXiv:** [2605.22138v1](https://arxiv.org/abs/2605.22138v1) · 2026-05-21 · cs.AI
**Authors:** Mingkai Deng, Jinyu Hou, Lara Sá Neves, Varad Pimpalkhute et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
How should an agent decide when and how to plan? A dominant approach builds agents as reactive policies with adaptive computation (e.g., chain-of-thought), trained end-to-end expecting planning to emerge implicitly. Without control over the presence, structure, or horizon of planning, these systems dramatically increase reasoning length, yielding inefficient token use without reliable accuracy gains. We argue efficient agentic reasoning benefits from decomposing decision-making into three systems: simulative reasoning (System II) grounding deliberation in future-state prediction via a world model; self-regulation (System III) deciding when and how deeply to plan via a learned configurator; and reactive execution (System I) handling fine-grained action. Simulative reasoning provides unified planning across diverse tasks without per-domain engineering, while self-regulation ensures the planner is invoked only when needed. To test this, we develop SR$^2$AM (Self-Regulated Simulative Reasoning Agentic LLM), realizing both as distinct stages within an LLM's chain-of-thought, with the LLM as world model. We explore two instantiations: recording decisions from a prompted multi-module system (v0.1) and reconstructing structured plans from traces of pretrained reasoning LLMs (v1.0), trained via supervised then reinforcement learning (RL). Across math, science, tabular analysis, and web information seeking, v0.1-8B and v1.0-30B achieve Pass@1 competitive with 120-355B and 685B-1T parameter systems respectively, while v1.0-30B uses 25.8-95.3% fewer reasoning tokens than comparable agentic LLMs. RL increases average planning horizon by 22.8% while planning frequency grows only 2.0%, showing it learns to plan further ahead rather than more often. More broadly, learned self-regulation instantiates a principle we expect to extend beyond planning to how agents govern their own learning and adaptation.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.22138v1)
