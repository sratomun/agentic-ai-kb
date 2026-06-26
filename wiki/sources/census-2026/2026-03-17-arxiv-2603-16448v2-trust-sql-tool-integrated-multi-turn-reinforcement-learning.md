---
type: source
source_type: arxiv
title: "TRUST-SQL: Tool-Integrated Multi-Turn Reinforcement Learning for Text-to-SQL over Unknown Schemas"
authors: Ai Jian, Xiaoyun Zhang, Wanrou Du, Jingqing Ruan et al.
url: https://arxiv.org/abs/2603.16448v2
date: 2026-03-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [data-query-agents, agentic-rl, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# TRUST-SQL: Tool-Integrated Multi-Turn Reinforcement Learning for Text-to-SQL over Unknown Schemas

**arXiv:** [2603.16448v2](https://arxiv.org/abs/2603.16448v2) · 2026-03-17 · cs.AI
**Authors:** Ai Jian, Xiaoyun Zhang, Wanrou Du, Jingqing Ruan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text-to-SQL parsing has achieved remarkable progress under the Full Schema Assumption. However, this premise fails in real-world enterprise environments where databases contain hundreds of tables with massive noisy metadata. Rather than injecting the full schema upfront, an agent must actively identify and verify only the relevant subset, giving rise to the Unknown Schema scenario we study in this work. To address this, we propose TRUST-SQL (Truthful Reasoning with Unknown Schema via Tools). We formulate the task as a Partially Observable Markov Decision Process where our autonomous agent employs a structured four-phase protocol to ground reasoning in verified metadata. Crucially, this protocol provides a structural boundary for our novel Dual-Track GRPO strategy. By applying token-level masked advantages, this strategy isolates exploration rewards from execution outcomes to resolve credit assignment, yielding a 9.9% relative improvement over standard GRPO. Extensive experiments across five benchmarks demonstrate that TRUST-SQL achieves an average absolute improvement of 30.6% and 16.6% for the 4B and 8B variants respectively over their base models. Remarkably, despite operating entirely without pre-loaded metadata, our framework consistently matches or surpasses strong baselines that rely on schema prefilling.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[grpo]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.16448v2)
