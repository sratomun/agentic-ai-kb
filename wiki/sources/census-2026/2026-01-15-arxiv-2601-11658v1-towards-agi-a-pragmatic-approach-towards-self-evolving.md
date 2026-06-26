---
type: source
source_type: arxiv
title: "Towards AGI A Pragmatic Approach Towards Self Evolving Agent"
authors: Indrajit Kar, Sammy Zonunpuia, Zonunfeli Ralte
url: https://arxiv.org/abs/2601.11658v1
date: 2026-01-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.CL
tags: [agent-reliability, self-evolving-agents, agentic-rl, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Towards AGI A Pragmatic Approach Towards Self Evolving Agent

**arXiv:** [2601.11658v1](https://arxiv.org/abs/2601.11658v1) · 2026-01-15 · cs.CL
**Authors:** Indrajit Kar, Sammy Zonunpuia, Zonunfeli Ralte

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Model (LLM) based agents are powerful yet fundamentally static after deployment, lacking the ability to autonomously expand capabilities, generate new tools, or evolve their reasoning. This work introduces a hierarchical self-evolving multi-agent framework that integrates a Base LLM, an operational SLM agent, a Code-Generation LLM, and a Teacher-LLM to enable continuous adaptation. The workflow begins with the agent attempting a task using reasoning and existing tools; if unsuccessful, it escalates to tool synthesis through the Code-Gen LLM, and when failures persist, it triggers an evolution phase using Curriculum Learning (CL), Reward-Based Learning (RL), or Genetic Algorithm (GA) evolution. Using the TaskCraft dataset rich in hierarchical tasks, tool-use traces, and difficulty scaling we evaluate these paradigms. CL delivers fast recovery and strong generalization, RL excels on high-difficulty tasks, and GA offers high behavioral diversity. Across all settings, evolved agents outperform their originals, demonstrating robust, autonomous, self-improving agentic evolution.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.11658v1)
