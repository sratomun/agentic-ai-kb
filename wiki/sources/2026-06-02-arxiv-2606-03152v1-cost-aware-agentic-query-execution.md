---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Cost-Aware Optimization for Agentic Query Execution"
authors: Lunyiu Nie, Yilin Xia, Yiren Liu, Christopher Jermaine, Swarat Chaudhuri (UT Austin; UIUC; Rice)
url: https://arxiv.org/abs/2606.03152
date: 2026-06-02
citationCount: 0
influentialCitationCount: 0
velocity: recent
ingested: 2026-06-26
tags: [arxiv, agent-finops, data-query-agents, text-to-sql, agentic-ai, 2026]
---

# Cost-Aware Optimization for Agentic Query Execution

**arXiv [2606.03152](https://arxiv.org/abs/2606.03152)** · 2026-06-02 · **recent** (PVLDB format) · Lunyiu Nie, Yilin Xia, Yiren Liu, Christopher Jermaine, Swarat Chaudhuri

**Significance.** Brings classical query optimization into the agent loop — the "optimize the plan" layer of [[agent-finops]], and a direct tie to [[data-query-agents]] / [[text-to-sql]].

## Abstract
Classical query optimization searches over algebraically equivalent plans that differ only in cost. This assumption breaks once LLM-backed operators enter the picture: their placement, ordering, and granularity jointly determine both dollar cost and answer quality, and the right choice among the alternatives is often revealed only at runtime. We formalize this setting as agentic query execution, a query execution paradigm in which agent-based planning is interleaved with execution, and agent workflow optimization becomes the analogue of classical query optimization. We then present EnumGRPO, a self-improving optimizer for this setting. During a learning stage, EnumGRPO enumerates query plans over decisions such as execution paradigm, operator type, operator placement, selectivity scope, and projection width, then distills quality-cost feedback into reusable planning heuristics via in-context reinforcement learning. Across four databases in SWAN, EnumGRPO achieves 35.4% execution accuracy at $0.011 per query in LLM-operator cost, a 317× cost reduction over the hybrid query baseline with an 18% relative improvement in answer accuracy.

## From the paper (full-text)
**Contribution / method.** Formalizes **agentic query execution** — interleaving LLM-operator planning with SQL execution over intermediate results, where structural choices jointly set cost AND correctness (no longer cost-neutral equivalences). **EnumGRPO** runs a learning stage that enumerates candidate workflows over five plan axes (execution paradigm, operator type, placement, selectivity scope, projection width), scores them on a joint quality-cost reward, uses **group-relative advantages (GRPO)** to separate structural effects from query difficulty, and distills contrastive feedback into **natural-language planning heuristics via in-context RL** — no weight updates, so heuristics are human-readable, auditable, and portable across model upgrades.
**Results.** **35.4% execution accuracy at $0.011/query** vs Agentic BlendSQL's $3.42/query — **~317× cost reduction** with an 18% relative accuracy gain. Over the unoptimized agentic base ($0.039/query), a further 72% cost cut while raising accuracy 32.1%→35.4% EX. LLM-operator token use falls **64.4%** (52K→18K tokens/query); latency 235s→153s. Cross-schema transfer holds accuracy (32.9% vs 32.1%) while cutting cost $3.11→$0.77; the learned pool converges to 32 plain-English heuristics (e.g., "prefer llm_reduce over per-row llm_map; 5–11× cheaper").
**Takeaway.** Let an agent enumerate-then-distill plan-level heuristics (push SQL filters before LLM calls; batch, don't go per-row) — LLM-in-the-loop analytics gets ~300× cheaper *and* more accurate, with heuristics that survive model upgrades.

## Graph
- **Concepts:** [[agent-finops|Agent FinOps]] · [[data-query-agents|Data-query agents]] · [[text-to-sql|Text-to-SQL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]]
- **Raw:** census record `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.03152v1); full text read via alphaXiv (https://arxiv.org/abs/2606.03152). Raw fulltext capture pending backfill.
