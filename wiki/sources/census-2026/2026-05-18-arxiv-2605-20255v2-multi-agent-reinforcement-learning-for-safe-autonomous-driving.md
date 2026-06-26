---
type: source
source_type: arxiv
title: "Multi-Agent Reinforcement Learning for Safe Autonomous Driving Under Pedestrian Behavioral Uncertainty"
authors: Prakash Aryan, Kaushik Raghupathruni, Timo Kehrer, Sebastiano Panichella
url: https://arxiv.org/abs/2605.20255v2
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 11
primary: cs.LG
tags: [autonomous-driving-agents, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Agent Reinforcement Learning for Safe Autonomous Driving Under Pedestrian Behavioral Uncertainty

**arXiv:** [2605.20255v2](https://arxiv.org/abs/2605.20255v2) · 2026-05-18 · cs.LG
**Authors:** Prakash Aryan, Kaushik Raghupathruni, Timo Kehrer, Sebastiano Panichella

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Simulation-based testing of self-driving cars (SDCs) typically relies on scripted pedestrian models that do not capture the heterogeneity and uncertainty of real crossing behavior, limiting the realism of safety assessments, especially for jaywalking, which is governed by latent personality traits the vehicle cannot observe. We hypothesize that jointly training pedestrians and the SDC with multi-agent reinforcement learning (MARL) yields more realistic interaction scenarios than training against fixed pedestrian policies, and that the behavior gap between predictable and unpredictable crossings can be measured directly from trajectories. We co-train an SDC and 12 pedestrians using Multi-Agent Proximal Policy Optimization (MAPPO): pedestrian locomotion follows scripted Dijkstra pathfinding while an RL policy controls high-level go/wait decisions, and jaywalking probability depends on a per-pedestrian trait sampled at episode start and hidden from the SDC. In 500-episode evaluations, the co-trained SDC reached 78% of goals with a 14% collision rate, versus 35%/33% for the best rule-based baseline. A speed differential metric shows the SDC traveled 2.65 m/s faster near jaywalkers than near crosswalk users at close range (0-3 m), indicating jaywalking encounters were not anticipated. Jaywalking was 13% of crossing events but 62% of collisions, and co-training reduced collisions by 30% relative to single-agent RL as pedestrians learned to wait when the SDC approached at speed.

## Graph
- **Concepts:** [[autonomous-driving-agents|Autonomous-driving agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.20255v2)
