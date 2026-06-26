---
type: source
source_type: arxiv
title: "Beyond the Black Box: Interpretability of Agentic AI Tool Use"
authors: Hariom Tatsat, Ariye Shater
url: https://arxiv.org/abs/2605.06890v3
date: 2026-05-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, agent-reliability, agent-security, agent-memory, tool-use, arxiv, auto-ingested]
---

# Beyond the Black Box: Interpretability of Agentic AI Tool Use

**arXiv:** [2605.06890v3](https://arxiv.org/abs/2605.06890v3) · 2026-05-07 · cs.AI
**Authors:** Hariom Tatsat, Ariye Shater

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
AI agents are promising for high-stakes enterprise workflows, but dependable deployment remains limited because tool-use failures are difficult to diagnose and control. Agents may skip required tool calls, invoke tools unnecessarily, or take actions whose consequence becomes visible only after execution. Existing observability methods are external: prompts reveal correlations, evaluations score outputs, and logs arrive only after the model has already acted. In long-horizon settings, these failures are costly because an early tool mistake can alter the rest of the trajectory, increase token consumption, and create downstream safety and security risk. We introduce a mechanistic-interpretability toolkit built on Sparse Autoencoders (SAEs), which decompose activations into sparse internal features, and linear probes, lightweight classifiers that read signals from those features. The framework reads model states before each action and infers whether a tool is needed and how risky the next tool action is. It identifies the model layers and features most associated with tool decisions and tests their functional importance through feature ablation. We train the probes on multi-step trajectories from the NVIDIA Nemotron function-calling dataset and apply the same workflow to GPT-OSS 20B and Gemma 3 27B models. The goal is not to replace external evaluation, but to add a missing layer: visibility into what the model signaled internally before action. This helps surface deeper causes of agent failure, especially in long-horizon runs where an early mistake can impact subsequent agent behavior. More broadly, the paper shows how mechanistic interpretability can support internal observability for monitoring tool calls and risk in agent systems.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.06890v3)
