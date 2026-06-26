---
type: source
source_type: arxiv
title: "SelfHeal: Empirical Fix Pattern Analysis and Bug Repair in LLM Agents"
authors: Niful Islam, Muhammad Anas Raza, Mohammad Wardat
url: https://arxiv.org/abs/2604.17699v1
date: 2026-04-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SelfHeal: Empirical Fix Pattern Analysis and Bug Repair in LLM Agents

**arXiv:** [2604.17699v1](https://arxiv.org/abs/2604.17699v1) · 2026-04-20 · cs.SE
**Authors:** Niful Islam, Muhammad Anas Raza, Mohammad Wardat

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models (LLMs) have transformed software development and AI applications. While LLMs are designed for text processing, LLM agents extend this capability by enabling autonomous actions, tool use, and multi-step task completion. As this field grows, developers face new challenges in debugging these complex systems. To address this challenge, we present the first empirical study on bug fix patterns in LLM agents. We study buggy posts and code snippets from three platforms: Stack Overflow, GitHub, and HuggingFace Forums. We examine their fix patterns, the components where fixes are applied, and the programming languages and frameworks involved. Furthermore, we introduce AgentDefect, the first benchmark dataset for bugs in LLM agents. The dataset contains 37 runtime buggy instances along with fixed code and test files. Finally, we present SelfHeal, a multi-agent system designed to fix bugs in LLM agents. The system leverages two independent ReAct agents: the fix agent and the critic agent. These agents use tools that provide both internal knowledge (fix rules) and external knowledge (web search) to propose and validate fixes. Our evaluation shows that SelfHeal with Gemini 3 Pro as the backbone LLM outperforms both baseline and state-of-the-art approaches by a significant margin.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.17699v1)
