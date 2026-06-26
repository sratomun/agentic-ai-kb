---
type: source
source_type: arxiv
title: "SEVerA: Verified Synthesis of Self-Evolving Agents"
authors: Debangshu Banerjee, Changming Xu, Eugene Ie, Ming Zhang et al.
url: https://arxiv.org/abs/2603.25111v2
date: 2026-03-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.LG
tags: [coding-agents, science-agents, agent-reliability, self-evolving-agents, agentic-rl, arxiv, auto-ingested]
---

# SEVerA: Verified Synthesis of Self-Evolving Agents

**arXiv:** [2603.25111v2](https://arxiv.org/abs/2603.25111v2) · 2026-03-26 · cs.LG
**Authors:** Debangshu Banerjee, Changming Xu, Eugene Ie, Ming Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances have shown the effectiveness of self-evolving LLM agents on tasks such as program repair and scientific discovery. In this paradigm, a planner LLM synthesizes an agent program that invokes parametric models, including LLMs, which are then tuned per task to improve performance. However, existing self-evolving agent frameworks provide no formal guarantees of safety or correctness. Because such programs are often executed autonomously on unseen inputs, this lack of guarantees raises reliability and security concerns. We formulate agentic code generation as a constrained learning problem, combining hard formal specifications with soft objectives capturing task utility. We introduce Formally Guarded Generative Models (FGGM), which allow the planner LLM to specify a formal output contract for each generative model call using first-order logic. Each FGGM call wraps the underlying model in a rejection sampler with a verified fallback, ensuring every returned output satisfies the contract for any input and parameter setting. Building on FGGM, we present SEVerA (Self-Evolving Verified Agents), a three-stage framework: Search synthesizes candidate parametric programs containing FGGM calls; Verification proves correctness with respect to hard constraints for all parameter values, reducing the problem to unconstrained learning; and Learning applies scalable gradient-based optimization, including GRPO-style fine-tuning, to improve the soft objective while preserving correctness. We evaluate SEVerA on Dafny program verification, symbolic math synthesis, and policy-compliant agentic tool use ($τ^2$-bench). Across tasks, SEVerA achieves zero constraint violations while improving performance over unconstrained and SOTA baselines, showing that formal behavioral constraints not only guarantee correctness but also steer synthesis toward higher-quality agents.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.25111v2)
