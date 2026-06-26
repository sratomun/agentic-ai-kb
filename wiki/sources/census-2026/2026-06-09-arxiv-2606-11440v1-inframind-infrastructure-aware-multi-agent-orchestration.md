---
type: source
source_type: arxiv
title: "INFRAMIND: Infrastructure-Aware Multi-Agent Orchestration"
authors: Ahasan Kabir, Jiaqi Xue, Mengxin Zheng, Qian Lou
url: https://arxiv.org/abs/2606.11440v1
date: 2026-06-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, multi-agent-systems, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# INFRAMIND: Infrastructure-Aware Multi-Agent Orchestration

**arXiv:** [2606.11440v1](https://arxiv.org/abs/2606.11440v1) · 2026-06-09 · cs.AI
**Authors:** Ahasan Kabir, Jiaqi Xue, Mengxin Zheng, Qian Lou

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing multi-agent LLM orchestration methods, ranging from brute-force ensembles to learned routers, select models and topologies based on task and model features. However, these methods do not consider the runtime state of the serving infrastructure. On shared GPU clusters under concurrent load, this infrastructure blindness causes systematic resource underutilization: preferred models accumulate deep request queues while equally capable alternatives sit idle. In multi-agent pipelines, where each query triggers multiple sequential model calls, these delays then compound across every downstream step. Closing this gap is challenging because the relevant infrastructure signals (queue depths, KV-cache pressure, latencies) are dynamic and noisy, and they must drive three different decisions: planning, per-step routing, and scheduling. We introduce INFRAMIND, a framework that makes the entire multi-agent stack infrastructure-aware. An infra-aware planner conditions topology and role selection on real-time system load and remaining budget, biasing toward simpler graphs under congestion and richer ones at low load. An infra-aware executor then observes per-model queue depths, cache utilization, and response latencies at each agent step to decide which model to call and how deeply to reason; a budget-aware scheduler further reorders each model's queue so that urgent requests are served first. Cast as a hierarchical constrained MDP and solved end-to-end via reinforcement learning, the system learns to balance quality against latency automatically. Across five benchmarks, INFRAMIND delivers up to +7.6 pp accuracy over the prior baseline at low load with up to 7x lower latency, and sustains up to 99.9% SLO compliance under high load where every baseline drops below 50%.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.11440v1)
