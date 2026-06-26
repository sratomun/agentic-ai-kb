---
type: source
source_type: arxiv
title: "Agent-Omit: Adaptive Context Omission for Efficient LLM Agents"
authors: Yansong Ning, Jun Fang, Naiqiang Tan, Hao Liu
url: https://arxiv.org/abs/2602.04284v2
date: 2026-02-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.AI
tags: [agentic-rl, agent-evaluation, arxiv, auto-ingested]
---

# Agent-Omit: Adaptive Context Omission for Efficient LLM Agents

**arXiv:** [2602.04284v2](https://arxiv.org/abs/2602.04284v2) · 2026-02-04 · cs.AI
**Authors:** Yansong Ning, Jun Fang, Naiqiang Tan, Hao Liu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Managing agent context (e.g., thought and observation) during multi-turn agent-environment interactions is an emerging strategy to improve agent efficiency. However, existing studies treat the entire interaction trajectories equally, overlooking the thought necessity and observation utility varies across turns. To this end, we first conduct quantitative investigations into how thought and observation affect agent effectiveness and efficiency. Based on our findings, we propose Agent-Omit, a unified training framework that empowers LLM agents to adaptively omit redundant thoughts and observations. Specifically, we first synthesize a small amount of cold-start data, including both single-turn and multi-turn omission scenarios, to fine-tune the agent for omission behaviors. Furthermore, we introduce an omit-aware agentic reinforcement learning approach, incorporating a dual sampling mechanism and a tailored omission reward to incentivize the agent's adaptive omission capability. Theoretically, we prove that the deviation of our omission policy is upper-bounded by KL-divergence. Experimental results on five agent benchmarks show that our constructed Agent-Omit-8B could obtain performance comparable to seven frontier LLM agent, and achieve the best effectiveness-efficiency trade-off than seven efficient LLM agents methods. Our code and data are available at https://github.com/usail-hkust/Agent-Omit.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.04284v2)
