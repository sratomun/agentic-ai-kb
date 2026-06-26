---
type: source
source_type: arxiv
title: "Just Ask: Curious Code Agents Reveal System Prompts in Frontier LLMs"
authors: Xiang Zheng, Yutao Wu, Hanxun Huang, Yige Li et al.
url: https://arxiv.org/abs/2601.21233v1
date: 2026-01-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [coding-agents, agent-reliability, self-evolving-agents, agent-security, agent-skills, arxiv, auto-ingested]
---

# Just Ask: Curious Code Agents Reveal System Prompts in Frontier LLMs

**arXiv:** [2601.21233v1](https://arxiv.org/abs/2601.21233v1) · 2026-01-29 · cs.AI
**Authors:** Xiang Zheng, Yutao Wu, Hanxun Huang, Yige Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous code agents built on large language models are reshaping software and AI development through tool use, long-horizon reasoning, and self-directed interaction. However, this autonomy introduces a previously unrecognized security risk: agentic interaction fundamentally expands the LLM attack surface, enabling systematic probing and recovery of hidden system prompts that guide model behavior. We identify system prompt extraction as an emergent vulnerability intrinsic to code agents and present \textbf{\textsc{JustAsk}}, a self-evolving framework that autonomously discovers effective extraction strategies through interaction alone. Unlike prior prompt-engineering or dataset-based attacks, \textsc{JustAsk} requires no handcrafted prompts, labeled supervision, or privileged access beyond standard user interaction. It formulates extraction as an online exploration problem, using Upper Confidence Bound-based strategy selection and a hierarchical skill space spanning atomic probes and high-level orchestration. These skills exploit imperfect system-instruction generalization and inherent tensions between helpfulness and safety. Evaluated on \textbf{41} black-box commercial models across multiple providers, \textsc{JustAsk} consistently achieves full or near-complete system prompt recovery, revealing recurring design- and architecture-level vulnerabilities. Our results expose system prompts as a critical yet largely unprotected attack surface in modern agent systems.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-security|Agent security]] · [[agent-skills|Agent skills]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.21233v1)
