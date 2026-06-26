---
type: source
source_type: arxiv
title: "Spider-Sense: Intrinsic Risk Sensing for Efficient Agent Defense with Hierarchical Adaptive Screening"
authors: Zhenxiong Yu, Zhi Yang, Zhiheng Jin, Shuhe Wang et al.
url: https://arxiv.org/abs/2602.05386v2
date: 2026-02-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.CR
tags: [agent-security, agent-evaluation, arxiv, auto-ingested]
---

# Spider-Sense: Intrinsic Risk Sensing for Efficient Agent Defense with Hierarchical Adaptive Screening

**arXiv:** [2602.05386v2](https://arxiv.org/abs/2602.05386v2) · 2026-02-05 · cs.CR
**Authors:** Zhenxiong Yu, Zhi Yang, Zhiheng Jin, Shuhe Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As large language models (LLMs) evolve into autonomous agents, their real-world applicability has expanded significantly, accompanied by new security challenges. Most existing agent defense mechanisms adopt a mandatory checking paradigm, in which security validation is forcibly triggered at predefined stages of the agent lifecycle. In this work, we argue that effective agent security should be intrinsic and selective rather than architecturally decoupled and mandatory. We propose Spider-Sense framework, an event-driven defense framework based on Intrinsic Risk Sensing (IRS), which allows agents to maintain latent vigilance and trigger defenses only upon risk perception. Once triggered, the Spider-Sense invokes a hierarchical defence mechanism that trades off efficiency and precision: it resolves known patterns via lightweight similarity matching while escalating ambiguous cases to deep internal reasoning, thereby eliminating reliance on external models. To facilitate rigorous evaluation, we introduce S$^2$Bench, a lifecycle-aware benchmark featuring realistic tool execution and multi-stage attacks. Extensive experiments demonstrate that Spider-Sense achieves competitive or superior defense performance, attaining the lowest Attack Success Rate (ASR) and False Positive Rate (FPR), with only a marginal latency overhead of 8.3\%.

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[spider-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.05386v2)
