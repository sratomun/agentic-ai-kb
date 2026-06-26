---
type: source
source_type: arxiv
title: "Solvita: Enhancing Large Language Models for Competitive Programming via Agentic Evolution"
authors: Han Li, Jinyu Tian, Rili Feng, Yuqiao Du et al.
url: https://arxiv.org/abs/2605.15301v1
date: 2026-05-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [agent-reliability, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# Solvita: Enhancing Large Language Models for Competitive Programming via Agentic Evolution

**arXiv:** [2605.15301v1](https://arxiv.org/abs/2605.15301v1) · 2026-05-14 · cs.AI
**Authors:** Han Li, Jinyu Tian, Rili Feng, Yuqiao Du et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) still struggle with the rigorous reasoning demands of hard competitive programming. While recent multi-agent frameworks attempt to bridge this reliability gap, they remain fundamentally stateless: they rely on static retrieval and discard the valuable problem-solving and debugging experience gained from previous tasks. To address this, we present Solvita, an agentic evolution framework that enables continuous learning without requiring weight updates to the underlying LLM. Solvita reorganizes problem-solving into a closed-loop system of strategy selection, program synthesis, certified supervision, and targeted hacking, executed by four specialized agents: Planner, Solver, Oracle, and Hacker. Crucially, each agent is paired with a trainable, graph-structured knowledge network. As the system operates, outcome signals, such as pass/fail verdicts, test certification quality, and adversarial vulnerabilities discovered by the Hacker, are recast as reinforcement learning updates to these network weights. This allows the agents to dynamically route future queries based on past successes and failures, effectively accumulating transferable reasoning experience over time. Evaluated across CodeContests, APPS, AetherCode, and live Codeforces rounds, Solvita establishes a new state-of-the-art among code-generation agents, outperforming existing multi-agent pipelines and nearly doubling the accuracy of single-pass baselines.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15301v1)
