---
type: source
source_type: arxiv
title: "STAR-PólyaMath: Multi-Agent Reasoning under Persistent Meta-Strategic Supervision"
authors: Jiaao Wu, Xian Zhang, Hanzhang Liu, Sophia Zhang et al.
url: https://arxiv.org/abs/2605.19338v1
date: 2026-05-19
ingested: 2026-06-21
depth: abstract
auto: true
score: 24
primary: cs.MA
tags: [agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# STAR-PólyaMath: Multi-Agent Reasoning under Persistent Meta-Strategic Supervision

**arXiv:** [2605.19338v1](https://arxiv.org/abs/2605.19338v1) · 2026-05-19 · cs.MA
**Authors:** Jiaao Wu, Xian Zhang, Hanzhang Liu, Sophia Zhang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Frontier AI models and multi-agent systems have led to significant improvements in mathematical reasoning. However, for problems requiring extended, long-horizon reasoning, existing systems continue to suffer from fundamental reliability issues: hallucination accumulation, memory fragmentation, and imbalanced reasoning-tool trade-offs. In this paper, we introduce STAR-PólyaMath, a multi-agent framework that systematically addresses these challenges through meta-level supervision and structured Reasoner-Verifier interaction. STAR-PólyaMath is structured as an orchestrated state machine with nested challenge-step-replan loops, governed by a reasoning-free Python orchestrator that separates control from inference and bounds error propagation through trace-back and re-planning. Our key innovation is a persistent Meta-Strategist that maintains cross-attempt memory and exercises meta-level control by issuing high-level strategic guidance or mandatory directives, so the system can escape unproductive loops rather than stagnate or over-rely on tools. STAR-PólyaMath achieves state-of-the-art results on all eight top-tier competition benchmarks: AIME 2025-2026, MathArena Apex Shortlist, MathArena Apex 2025, Putnam 2025, IMO 2025, HMMT February 2026, and USAMO 2026. It obtains perfect scores on AIMEs, Putnam, and HMMT, and shows its largest margin on Apex 2025, scoring 93.75% compared with 80.21% by the strongest baseline GPT-5.5. Ablation studies show that the gains arise from the framework's orchestration rather than from model-level diversity since removing key components or substituting in mixed backbones consistently weakens performance. Code is available at https://github.com/Julius-Woo/STAR-PolyaMath.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.19338v1)
