---
type: source
source_type: arxiv
title: "HIPIF: Hierarchical Planning and Information Folding for Long-Horizon LLM Agent Learning"
authors: Juncheng Diao, Zhicong Lu, Peiguang Li, Yongwei Zhou et al.
url: https://arxiv.org/abs/2606.10507v1
date: 2026-06-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# HIPIF: Hierarchical Planning and Information Folding for Long-Horizon LLM Agent Learning

**arXiv:** [2606.10507v1](https://arxiv.org/abs/2606.10507v1) · 2026-06-09 · cs.AI
**Authors:** Juncheng Diao, Zhicong Lu, Peiguang Li, Yongwei Zhou et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While Large Language Models (LLMs) have demonstrated strong capabilities as autonomous agents across a wide range of tasks, their performance often degrades in multi-turn long-horizon agentic tasks. Existing methods have made progress through fine-grained credit assignment to alleviate long-horizon sparse rewards and hierarchical reinforcement learning to decompose tasks and reduce long-term dependency. However, these methods still do not directly address long-context interference, in which continuously growing histories weaken the agent's ability to track the global task state and impair subsequent reasoning and decision-making. Inspired by the way humans handle complex tasks through subgoal decomposition and completed progress summarization, we propose Hierarchical Planning and Information Folding (HIPIF) for long-horizon LLM agent learning. HIPIF trains the agent end-to-end to organize long-horizon execution around explicit subgoals while folding completed subgoal histories to reduce long-context interference. Furthermore, to stabilize subgoal-based planning and execution, HIPIF combines hierarchical reflection and subgoal-oriented process rewards to guide subgoal generation, transition, and execution, without relying on costly auxiliary models or task-specific expert trajectories. Extensive experiments on three publicly available agentic benchmarks demonstrate the validity of our method.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.10507v1)
