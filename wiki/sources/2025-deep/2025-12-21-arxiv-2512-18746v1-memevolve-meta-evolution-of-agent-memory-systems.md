---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MemEvolve: Meta-Evolution of Agent Memory Systems"
authors: Guibin Zhang, Haotian Ren, Chong Zhan, Zhenhong Zhou et al.
url: https://arxiv.org/abs/2512.18746v1
date: 2025-12-21
citationCount: 52
influentialCitationCount: 3
velocity: 8.65
ingested: 2026-06-22
tags: [self-evolving-agents, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MemEvolve: Meta-Evolution of Agent Memory Systems

**arXiv [2512.18746v1](https://arxiv.org/abs/2512.18746v1)** · 2025-12-21 · **52 citations** (3 influential · 8.65/mo) · Guibin Zhang, Haotian Ren, Chong Zhan, Zhenhong Zhou et al.

## Abstract
Self-evolving memory systems are unprecedentedly reshaping the evolutionary paradigm of large language model (LLM)-based agents. Prior work has predominantly relied on manually engineered memory architectures to store trajectories, distill experience, and synthesize reusable tools, enabling agents to evolve on the fly within environment interactions. However, this paradigm is fundamentally constrained by the staticity of the memory system itself: while memory facilitates agent-level evolving, the underlying memory architecture cannot be meta-adapted to diverse task contexts. To address this gap, we propose MemEvolve, a meta-evolutionary framework that jointly evolves agents' experiential knowledge and their memory architecture, allowing agent systems not only to accumulate experience but also to progressively refine how they learn from it. To ground MemEvolve in prior research and foster openness in future self-evolving systems, we introduce EvolveLab, a unified self-evolving memory codebase that distills twelve representative memory systems into a modular design space (encode, store, retrieve, manage), providing both a standardized implementation substrate and a fair experimental arena. Extensive evaluations on four challenging agentic benchmarks demonstrate that MemEvolve achieves (I) substantial performance gains, improving frameworks such as SmolAgent and Flash-Searcher by up to $17.06\%$; and (II) strong cross-task and cross-LLM generalization, designing memory architectures that transfer effectively across diverse benchmarks and backbone models.

## From the paper (full-text excerpts)
**Introduction.** Introduction Language agents and agent systems, empowered by increasingly capable foundation models (Team et al., 2025a,b) and sophisticated scaffolding (Wang et al., 2024a; LangChain, 2023), have advanced rapidly, demonstrating unprecedented performance across complex tasks such as deep research (Chen et al., 2025), scientific discovery (Bai et al., 2025; Wei et al., 2025b), and industrial report generation (Zhang et al., 2025g). A key driving force behind this success is the agent memory system (Zhang et al., 2024b; Hu et al., 2025c), which persistently captures interactions between the agent and environment, distilling them into diverse forms of knowledge and skills, and thereby enabling large language model (LLM)-based agents to evolve continuously in task solving and world exploration (Wu et al., 2025c). Naturally, the choice of memory paradigm plays a decisive role in shaping an agent’s capacity for on-the-fly selfevolution. Initial designs centered on raw trajectory storage and few-shot prompting (Zhong et al., 2024; Wen et al., 2024), which were later superseded by more abst…

**Method / approach.** approaches share the same ambition, i.e., to enable agents to learn, adapt, and improve in a human-esque manner. 3 EvolveLab: A Unified Codebase for Self-Evolving Memory In this section, we first formalize the LLM-based agentic system and its associated memory architecture, then present the modular design space of EvolveLab, which comprehensively captures the characteristics of existing self-evolving agent memories, and finally introduce the unified codebase EvolveLab. 3.1 Preliminary We formalize an LLM-based agentic system as M = ⟨I, S, A, Ψ, Ω⟩, where I indexes the {1, ⋯, N } agents, S denotes the shared state space, A = ⋃i∈I Ai represents the joint action space, and Ψ(st+1 ∣ st , at , µ(t)) describes the environment dynamics with µ(t) ∈ I indicating the active agent at time step t. The system leverages a memory module Ω, which maintains a continuously evolving memory state Mt . At each step, the active agent observes the current state st , considers a task-specific query Q, a…

**Results.** experimental arena. Extensive evaluations on four challenging agentic benchmarks demonstrate that MemEvolve achieves (I) substantial performance gains, improving frameworks such as SmolAgent and Flash-Searcher by up to 17.06%; and (II) strong cross-task and cross-LLM generalization, designing memory architectures that transfer effectively across diverse benchmarks and backbone models.  Date: December 23, 2025  Code: https://github.com/bingreeky/MemEvolve xbench-DS WebWalkerQA GAIA Figure 1 The comparison between MemEvolve and several popular self-evolving agent memory systems across benchmarks. The underlying framework is Flash-Searcher (Qin et al., 2025)+GPT-5-Mini. 1 Human Learners Evaluate $(1+2i)6-3i$. The answer seems to be 6-9i. Tasks d ar sg Solutions Di Tasks Evaluate $(1+2i)6-3i$. Solutions Task Solution The answer seems to be 6-9i. Feedback: Solution Solution Template Error Notebook Mediocre Learner on…

**Conclusion.** Conclusion This work provides a unified implementation and design space for the rapidly growing field of self-evolving agent memory, together with a standardized codebase, termed EvolveLab, upon which we further build MemEvolve, a meta-evolutionary memory framework. Departing from the conventional paradigm of manually crafting a single self-improving memory architecture and expecting it to generalize across all domains, MemEvolve instead embraces adaptive, architecture-level evolution driven by empirical interaction feedback. Extensive experiments across diverse agentic benchmarks and backbone models demonstrate the effectiveness, robustness, and generalization of this approach. Moreover, analysis of the automatically evolved memory system…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2512.18746v1.md` · `raw/arxiv/2512.18746v1.fulltext.md`
