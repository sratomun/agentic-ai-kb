---
type: source
source_type: arxiv
title: "SaaS-Bench: Can Computer-Use Agents Leverage Real-World SaaS to Solve Professional Workflows?"
authors: Kean Shi, Zihang Li, Tianyi Ma, Zengji Tu et al.
url: https://arxiv.org/abs/2605.15777v2
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [computer-use-agents, agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SaaS-Bench: Can Computer-Use Agents Leverage Real-World SaaS to Solve Professional Workflows?

**arXiv:** [2605.15777v2](https://arxiv.org/abs/2605.15777v2) · 2026-05-15 · cs.AI
**Authors:** Kean Shi, Zihang Li, Tianyi Ma, Zengji Tu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Computer-Using Agents (CUAs) are rapidly extending large language models (LLMs) beyond text-based reasoning toward action execution in more complex environments, such as web browsers and graphical user interfaces (GUIs). However, existing web and GUI agent benchmarks often rely on simplified settings, isolated tasks, or short-horizon interactions, making it difficult to assess capabilities of agents in realistic professional workflows. Software-as-a-Service (SaaS) environments are a natural choice for CUA evaluation, as they host a large share of modern digital work and naturally involve dynamic system states, cross-application coordination, domain-specific knowledge, and long-horizon dependencies. To this end, we introduce SaaS-Bench, a benchmark built on 23 deployable SaaS systems across six professional domains, containing 106 tasks grounded in realistic work scenarios. These tasks require long-horizon execution, cover both text-only and multimodal settings, and are evaluated with weighted verification checkpoints that measure strict task completion and partial progress. Experiments show that representative LLM-based agents struggle on SaaS-Bench, with even the strongest model completing fewer than 4% of tasks end-to-end, exposing limitations in planning, state tracking, cross-application context maintenance, and error recovery. Code are available at https://github.com/UniPat-AI/SaaS-Bench for reproduction.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15777v2)
