---
type: source
source_type: arxiv
title: "AgentFugue: Agent Scaling for Long-Horizon Tasks through Collective Reasoning"
authors: Yuyang Hu, Hongjin Qian, Shuting Wang, Jiongnan Liu et al.
url: https://arxiv.org/abs/2605.24486v1
date: 2026-05-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agentic-rl, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# AgentFugue: Agent Scaling for Long-Horizon Tasks through Collective Reasoning

**arXiv:** [2605.24486v1](https://arxiv.org/abs/2605.24486v1) · 2026-05-23 · cs.AI
**Authors:** Yuyang Hu, Hongjin Qian, Shuting Wang, Jiongnan Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent progress on long-horizon agentic tasks has been driven largely by scaling up individual agents through stronger models, better tools, and more effective scaffolding. In contrast, much less is understood about scaling out: whether multiple peer agents, all targeting the same task, can become an additional source of capability without relying on explicit role specialization or workflow orchestration. We study this question and propose AgentFugue, a collective reasoning framework built around a shared reasoning hub. As peer agents explore the same task in parallel, the hub records concise notes on what each agent has established, attempted, or ruled out, and enables each agent to selectively access what other agents have discovered in a form useful for its current search. This design turns otherwise isolated trajectories into a connected ecology of reusable intermediate reasoning without requiring centralized planning. We instantiate the hub as a plug-in communication layer, trained with supervised fine-tuning and end-to-end reinforcement learning. Across the challenging long-horizon settings we study, AgentFugue improves over strong baselines. Our results suggest that collective reasoning can turn scaling out peer agent systems into a distinct source of capability gains, rather than merely a way of spending more compute.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.24486v1)
