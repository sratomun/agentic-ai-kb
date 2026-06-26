---
type: source
source_type: arxiv
title: "AnalogAgent: Self-Improving Analog Circuit Design Automation with LLM Agents"
authors: Zhixuan Bao, Zhuoyi Lin, Jiageng Wang, Jinhai Hu et al.
url: https://arxiv.org/abs/2603.23910v1
date: 2026-03-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, self-evolving-agents, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AnalogAgent: Self-Improving Analog Circuit Design Automation with LLM Agents

**arXiv:** [2603.23910v1](https://arxiv.org/abs/2603.23910v1) · 2026-03-25 · cs.AI
**Authors:** Zhixuan Bao, Zhuoyi Lin, Jiageng Wang, Jinhai Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in large language models (LLMs) suggest strong potential for automating analog circuit design. Yet most LLM-based approaches rely on a single-model loop of generation, diagnosis, and correction, which favors succinct summaries over domain-specific insight and suffers from context attrition that erases critical technical details. To address these limitations, we propose AnalogAgent, a training-free agentic framework that integrates an LLM-based multi-agent system (MAS) with self-evolving memory (SEM) for analog circuit design automation. AnalogAgent coordinates a Code Generator, Design Optimizer, and Knowledge Curator to distill execution feedback into an adaptive playbook in SEM and retrieve targeted guidance for subsequent generation, enabling cross-task transfer without additional expert feedback, databases, or libraries. Across established benchmarks, AnalogAgent achieves 92% Pass@1 with Gemini and 97.4% Pass@1 with GPT-5. Moreover, with compact models (e.g., Qwen-8B), it yields a +48.8% average Pass@1 gain across tasks and reaches 72.1% Pass@1 overall, indicating that AnalogAgent substantially strengthens open-weight models for high-quality analog circuit design automation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[qwen]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.23910v1)
