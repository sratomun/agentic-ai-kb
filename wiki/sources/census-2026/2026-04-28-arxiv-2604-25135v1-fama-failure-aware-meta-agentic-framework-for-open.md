---
type: source
source_type: arxiv
title: "FAMA: Failure-Aware Meta-Agentic Framework for Open-Source LLMs in Interactive Tool Use Environments"
authors: Amir Saeidi, Venkatesh Mishra, Souradeep Mukhopadhyay, Gaowen Liu et al.
url: https://arxiv.org/abs/2604.25135v1
date: 2026-04-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 26
primary: cs.CL
tags: [agent-reliability, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# FAMA: Failure-Aware Meta-Agentic Framework for Open-Source LLMs in Interactive Tool Use Environments

**arXiv:** [2604.25135v1](https://arxiv.org/abs/2604.25135v1) · 2026-04-28 · cs.CL
**Authors:** Amir Saeidi, Venkatesh Mishra, Souradeep Mukhopadhyay, Gaowen Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large Language Models are being increasingly deployed as the decision-making core of autonomous agents capable of effecting change in external environments. Yet, in conversational benchmarks, which simulate real-world customer-centric issue resolution scenarios, these agents frequently fail due to the cascading effects of incorrect decision-making. These challenges are particularly pronounced for open-source LLMs with smaller parameter sizes, limited context windows, and constrained inference budgets, which contribute to increased error accumulation in agentic settings. To tackle these challenges, we present the Failure-Aware Meta-Agentic (FAMA) framework. FAMA operates in two stages: first, it analyzes failure trajectories from baseline agents to identify the most prevalent errors; second, it employs an orchestration mechanism that activates a minimal subset of specialized agents tailored to address these failures by injecting a targeted context for the tool-use agent before the decision-making step. Experiments across open-source LLMs demonstrate performance gains up to 27% across evaluation modes over standard baselines. These results highlight that targeted curation of context through specialized agents to address common failures is a valuable design principle for building reliable, multi-turn tool-use LLM agents that simulate real-world conversational scenarios.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.25135v1)
