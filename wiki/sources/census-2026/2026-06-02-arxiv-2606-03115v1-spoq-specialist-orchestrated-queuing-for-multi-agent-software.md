---
type: source
source_type: arxiv
title: "SPOQ: Specialist Orchestrated Queuing for Multi-Agent Software Engineering"
authors: Royce Carbowitz, Dheeraj Kumar
url: https://arxiv.org/abs/2606.03115v1
date: 2026-06-02
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.SE
tags: [coding-agents, human-agent-interaction, multi-agent-systems, arxiv, auto-ingested]
---

# SPOQ: Specialist Orchestrated Queuing for Multi-Agent Software Engineering

**arXiv:** [2606.03115v1](https://arxiv.org/abs/2606.03115v1) · 2026-06-02 · cs.SE
**Authors:** Royce Carbowitz, Dheeraj Kumar

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-agent AI systems show promise for automating software engineering tasks, yet existing approaches suffer from coordination overhead, quality control gaps, and limited human oversight. We introduce SPOQ (Specialist Orchestrated Queuing), a methodology combining three innovations: (1) wave-based topological dispatch that computes parallel execution waves from task dependency graphs; (2) dual validation gates applying quality metrics before execution (planning validation) and after (code validation) to reduce rework cycles; and (3) Human-as-an-Agent (HaaA) integration, where a human specialist participates in decomposition and can be consulted during execution. SPOQ uses a three-tier agent hierarchy (Opus workers, Sonnet reviewers, Haiku investigators) to optimize cost-quality tradeoffs. We evaluate SPOQ through four experiments. Experiment 1: wave dispatch approaches the critical-path lower bound (ratio 1.03--1.11, speedup up to 14.3x); on a 2-slot local backend it delivers a stable 1.4x speedup. Experiment 2: SPOQ improves planning coverage from 93.0 to 99.75, eliminates cyclic plans, and lifts parallelism from 31.0 to 75.25. Experiment 3: dual validation reduces defects from 0.34 to 0.20 per task and lifts test pass rate from 91.25% to 99.75%. Experiment 4: human review reduces residual defects from 0.47 to 0.03 per task. Results are replicated on a locally hosted open-weights model (Qwen3.6-35B-A3B), verifying gains are attributable to orchestration rather than any specific model. A longitudinal study across 17 repositories, 8,589 commits, 1,822 tasks, and 13,866 tests (99.87% pass rate) provides ecological validation.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[human-agent-interaction|Human-agent interaction]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03115v1)
