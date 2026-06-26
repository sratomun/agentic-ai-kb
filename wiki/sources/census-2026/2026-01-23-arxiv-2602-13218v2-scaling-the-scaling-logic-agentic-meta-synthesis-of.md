---
type: source
source_type: arxiv
title: "Scaling the Scaling Logic: Agentic Meta-Synthesis of Logic Reasoning"
authors: Bowen Liu, Zhi Wu, Runquan Xie, Zhanhui Kang et al.
url: https://arxiv.org/abs/2602.13218v2
date: 2026-01-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [agentic-rl, agent-security, agent-protocols, arxiv, auto-ingested]
---

# Scaling the Scaling Logic: Agentic Meta-Synthesis of Logic Reasoning

**arXiv:** [2602.13218v2](https://arxiv.org/abs/2602.13218v2) · 2026-01-23 · cs.AI
**Authors:** Bowen Liu, Zhi Wu, Runquan Xie, Zhanhui Kang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Reinforcement Learning from Verifiable Rewards (RLVR) is bottlenecked by data: existing synthesis pipelines rely on expert-written code or fixed templates, confining growth to instance-level perturbations. We shift the evolvable unit from problem instances to task-family specifications. SSLogic is an agentic meta-synthesis framework in which LLM agents iteratively author and refine executable Generator-Validator pairs inside a closed Generate-Validate-Refine loop, producing families with new rules and difficulty gradients rather than parameter variations of old ones. A Multi-Gate Validation Protocol -- multi-strategy consensus plus Adversarial Blind Review, where independent agents solve each instance by writing and executing code -- filters ill-posed tasks before they enter training. Starting from 400 seed families, two evolution rounds yield 953 families and 21,389 verifiable instances. Three converging comparisons (step-matched, token-matched, and size-controlled on external Enigmata data) consistently show higher training utility of evolved data, with gains of SynLogic +5.2, AIME25 +3.0, and BBH +5.5 on Enigmata. Fine-grained KORBench evaluation reveals selective improvements in logic (+13.2%) and operation (+9.6%), linking structural evolution to downstream gains. Code: https://github.com/AdAstraAbyssoque/Scaling-the-Scaling-Logic

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.13218v2)
