---
type: source
source_type: arxiv
title: "Multi-Paradigm Agent Interaction in Practice:A Systematic Analysis of Generator-Evaluator, ReAct Loop,and Adversarial Evaluation in the buddyMe Framework"
authors: Xiaohua Wang, Chao Han, Kai Yu, XiaoLiang Xu et al.
url: https://arxiv.org/abs/2605.16821v1
date: 2026-05-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [agent-reliability, agent-security, agent-memory, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Paradigm Agent Interaction in Practice:A Systematic Analysis of Generator-Evaluator, ReAct Loop,and Adversarial Evaluation in the buddyMe Framework

**arXiv:** [2605.16821v1](https://arxiv.org/abs/2605.16821v1) · 2026-05-16 · cs.AI
**Authors:** Xiaohua Wang, Chao Han, Kai Yu, XiaoLiang Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The rapid evolution of Large Language Model (LLM) agents has produced diverse interaction paradigms, yet few production systems integrate multiple paradigms within a unified architecture. This paper presents a systematic analysis of three principal agent interaction paradigms, including Multi-Agent Orchestration (Generator-Evaluator), ReAct Tool-Use Loops, and Memory-Augmented Interaction, as implemented in buddyMe, an open-source multi-model agent programming framework. We formalize a five-stage processing pipeline: Requirement Pre-Review -> Task Decomposition -> ReAct Execution -> Real-Execution Verification -> Adversarial Evaluation Discussion, and establish a six-dimensional evaluation schema with weighted scoring. Through four empirical case studies drawn from real-world deployment logs covering museum guide generation, scheduled weather tasks, and comprehensive tour planning, we draw three key conclusions. First, Generator-Evaluator pre-review detects requirement omissions in 20 percent of complex tasks, with 80 percent tasks passing initial inspection. Second, the ReAct loop ensures stable subtask execution but leads to around 30 percent redundant tool invocations. Third, adversarial Evaluator-Defender discussions reach consensus within 2-3 rounds for nearly 70 percent of scenarios, functioning mainly for content refinement rather than logical reversal. We additionally provide three Mermaid-based architectural diagrams and conduct cross-paradigm comparisons with CrewAI, AutoGen, LangGraph, MemGPT and A-Mem across six system dimensions. The research outcomes offer practical design guidelines for constructing stable and reliable multi-paradigm agent systems.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[langgraph]] · [[autogen]] · [[crewai]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16821v1)
