---
type: source
source_type: arxiv
title: "Learning When to Act or Refuse: Guarding Agentic Reasoning Models for Safe Multi-Step Tool Use"
authors: Aradhye Agarwal, Gurdit Siyan, Yash Pandya, Joykirat Singh et al.
url: https://arxiv.org/abs/2603.03205v2
date: 2026-03-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.CL
tags: [agentic-rl, agent-security, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# Learning When to Act or Refuse: Guarding Agentic Reasoning Models for Safe Multi-Step Tool Use

**arXiv:** [2603.03205v2](https://arxiv.org/abs/2603.03205v2) · 2026-03-03 · cs.CL
**Authors:** Aradhye Agarwal, Gurdit Siyan, Yash Pandya, Joykirat Singh et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic language models operate in a fundamentally different safety regime than chat models: they must plan, call tools, and execute long-horizon actions where a single misstep, such as accessing files or entering credentials, can cause irreversible harm. Existing alignment methods, largely optimized for static generation and task completion, break down in these settings due to sequential decision-making, adversarial tool feedback, and overconfident intermediate reasoning. We introduce MOSAIC, a post-training framework that aligns agents for safe multi-step tool use by making safety decisions explicit and learnable. MOSAIC structures inference as a plan, check, then act or refuse loop, with explicit safety reasoning and refusal as first-class actions. To train without trajectory-level labels, we use preference-based reinforcement learning with pairwise trajectory comparisons, which captures safety distinctions often missed by scalar rewards. We evaluate MOSAIC zero-shot across three model families, Qwen2.5-7B, Qwen3-4B-Thinking, and Phi-4, and across out-of-distribution benchmarks spanning harmful tasks, prompt injection, benign tool use, and cross-domain privacy leakage. MOSAIC reduces harmful behavior by up to 50%, increases harmful-task refusal by over 20% on injection attacks, cuts privacy leakage, and preserves or improves benign task performance, demonstrating robust generalization across models, domains, and agentic settings.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.03205v2)
