---
type: source
source_type: arxiv
title: "SocialGrid: A Benchmark for Planning and Social Reasoning in Embodied Multi-Agent Systems"
authors: Hikaru Shindo, Hanzhao Lin, Lukas Helff, Patrick Schramowski et al.
url: https://arxiv.org/abs/2604.16022v1
date: 2026-04-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 23
primary: cs.AI
tags: [clinical-agents, embodied-agents, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SocialGrid: A Benchmark for Planning and Social Reasoning in Embodied Multi-Agent Systems

**arXiv:** [2604.16022v1](https://arxiv.org/abs/2604.16022v1) · 2026-04-17 · cs.AI
**Authors:** Hikaru Shindo, Hanzhao Lin, Lukas Helff, Patrick Schramowski et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As Large Language Models (LLMs) transition from text processors to autonomous agents, evaluating their social reasoning in embodied multi-agent settings becomes critical. We introduce SocialGrid, an embodied multi-agent environment inspired by Among Us that evaluates LLM agents on planning, task execution, and social reasoning. Our evaluations reveal that even the strongest open model (GPT-OSS-120B) achieves below 60% accuracy in task completion and planning, with agents getting stuck in repetitive behaviors or failing to navigate basic obstacles. Since poor navigation confounds evaluation of social intelligence, SocialGrid offers an optional Planning Oracle to isolate social reasoning from planning deficits. While planning assistance improves task completion, social reasoning remains a bottleneck: agents fail to detect deception at near-random chance regardless of scale, relying on shallow heuristics rather than accumulating behavioral evidence. SocialGrid provides automatic failure analysis and fine-grained metrics, enabling developers to diagnose and improve their agents. We also establish a competitive leaderboard using Elo ratings from adversarial league play.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[embodied-agents|Embodied agents]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.16022v1)
