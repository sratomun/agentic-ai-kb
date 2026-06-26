---
type: source
source_type: arxiv
title: "Beyond Monolithic Architectures: A Multi-Agent Search and Knowledge Optimization Framework for Agentic Search"
authors: Yiqun Chen, Lingyong Yan, Zixuan Yang, Erhan Zhang et al.
url: https://arxiv.org/abs/2601.04703v1
date: 2026-01-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agentic-rl, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Beyond Monolithic Architectures: A Multi-Agent Search and Knowledge Optimization Framework for Agentic Search

**arXiv:** [2601.04703v1](https://arxiv.org/abs/2601.04703v1) · 2026-01-08 · cs.AI
**Authors:** Yiqun Chen, Lingyong Yan, Zixuan Yang, Erhan Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic search has emerged as a promising paradigm for complex information seeking by enabling Large Language Models (LLMs) to interleave reasoning with tool use. However, prevailing systems rely on monolithic agents that suffer from structural bottlenecks, including unconstrained reasoning outputs that inflate trajectories, sparse outcome-level rewards that complicate credit assignment, and stochastic search noise that destabilizes learning. To address these challenges, we propose \textbf{M-ASK} (Multi-Agent Search and Knowledge), a framework that explicitly decouples agentic search into two complementary roles: Search Behavior Agents, which plan and execute search actions, and Knowledge Management Agents, which aggregate, filter, and maintain a compact internal context. This decomposition allows each agent to focus on a well-defined subtask and reduces interference between search and context construction. Furthermore, to enable stable coordination, M-ASK employs turn-level rewards to provide granular supervision for both search decisions and knowledge updates. Experiments on multi-hop QA benchmarks demonstrate that M-ASK outperforms strong baselines, achieving not only superior answer accuracy but also significantly more stable training dynamics.\footnote{The source code for M-ASK is available at https://github.com/chenyiqun/M-ASK.}

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.04703v1)
