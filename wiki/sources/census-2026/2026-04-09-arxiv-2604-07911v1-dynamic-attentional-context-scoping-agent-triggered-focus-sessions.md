---
type: source
source_type: arxiv
title: "Dynamic Attentional Context Scoping: Agent-Triggered Focus Sessions for Isolated Per-Agent Steering in Multi-Agent LLM Orchestration"
authors: Nickson Patel
url: https://arxiv.org/abs/2604.07911v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# Dynamic Attentional Context Scoping: Agent-Triggered Focus Sessions for Isolated Per-Agent Steering in Multi-Agent LLM Orchestration

**arXiv:** [2604.07911v1](https://arxiv.org/abs/2604.07911v1) · 2026-04-09 · cs.MA
**Authors:** Nickson Patel

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent LLM orchestration systems suffer from context pollution: when N concurrent agents compete for the orchestrator's context window, each agent's task state, partial outputs, and pending questions contaminate the steering interactions of every other agent, degrading decision quality. We introduce Dynamic Attentional Context Scoping (DACS), a mechanism in which the orchestrator operates in two asymmetric modes. In Registry mode it holds only lightweight per-agent status summaries (<=200 tokens each), remaining responsive to all agents and the user. When an agent emits a SteeringRequest, the orchestrator enters Focus(a_i) mode, injecting the full context of agent a_i while compressing all other agents to their registry entries. Context isolation is agent-triggered, asymmetric, and deterministic: the context window contains exactly F(a_i) + R_{-i} during steering, eliminating cross-agent contamination without requiring context compression or retrieval. We evaluate DACS across four experimental phases totalling 200 trials: Phase 1 tests N in {3,5,10} (60 trials); Phase 2 tests agent heterogeneity and adversarial dependencies (60 trials); Phase 3 tests decision density up to D=15 (40 trials); Phase 4 uses autonomous LLM agents for free-form questions (40 trials, Claude Haiku 4.5). Across all 8 synthetic scenarios, DACS achieves 90.0--98.4% steering accuracy versus 21.0--60.0% for a flat-context baseline (p < 0.0001 throughout), with wrong-agent contamination falling from 28--57% to 0--14% and context efficiency ratios of up to 3.53x. The accuracy advantage grows with N and D; keyword matching is validated by LLM-as-judge across all phases (mean kappa=0.909). DACS outperforms the flat-context baseline by +17.2pp at N=3 (p=0.0023) and +20.4pp at N=5 (p=0.0008) in Phase 4, with the advantage growing with N confirmed by two independent judges.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.07911v1)
