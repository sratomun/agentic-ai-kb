---
type: source
source_type: arxiv
title: "Both Ends Count! Just How Good are LLM Agents at 'Text-to-Big SQL'?"
authors: Germán T. Eizaguirre (URV), Lars Tissen (RWTH Aachen), Marc Sánchez-Artigas (URV)
url: https://arxiv.org/abs/2602.21480v4
date: 2026-02-25
ingested: 2026-06-22
depth: full-text
venue: EuroMLSys 2026
tags: [agent-evaluation, data-query-agents, arxiv]
---

# Both Ends Count! How Good are LLM Agents at "Text-to-Big SQL"?

**Why it matters:** The sharpest argument that **accuracy alone is the wrong metric for text2query at scale**. At Big-Data scale a minor translation error becomes a large cost/latency penalty, so eval must price execution efficiency and cost — and must count *both ends* (SQL generation latency + query execution). Introduces concrete cost/efficiency metrics that discriminate models that look identical on accuracy.

## What it is
A benchmarking methodology for text-to-Big-SQL agents (ReAct agent over Spark SQL with list/schema/check/run tools), evaluated on BIRD (accuracy) and TPC-H (deterministic data scaling, SF 10→1000). Tests frontier models (GPT-4o, GPT-5, GPT-5.2, Gemini 2.5/3 Flash, Gemini 3 Pro, Claude Opus 4.5/4.6, Kimi K2.5, GLM-5).

## Metrics (the contribution)
- **VES\*** — extends Valid Efficiency Score with column-level precision P(S,Ŝ) (penalizes superfluous columns) × end-to-end time ratio T_gold/T_e2e (counts agent reasoning + tool calls + query run, not just query run).
- **VCES** — VES\* divided by end-to-end cost (per-token billing + execution cost).
- **CVQ** — Expected Cost per Valid Query under retry-until-success = C_e2e / single-shot validity rate.

## Findings (verified)
- **Accuracy can't discriminate at the top:** on queries where models hit ~0.85+ EX, VES\* spreads them across an **809% range vs 54.93% for plain VES** — far sharper model selection.
- **Newer ≠ faster:** GPT-4o (2024) tops VES\* despite imperfect accuracy (0.93 EX); Claude Opus 4.6 reaches perfect accuracy but takes **92.37% longer** end-to-end than GPT-4o; Gemini 3 Pro / GLM-5 have poor, high-variance latency. The `check_query` (LLM-side) stage dominates end-to-end time.
- **Cost vs latency trade-off:** Gemini 3 Flash is the most cost-efficient (VCES) due to low per-token price; GPT-4o is latency-optimal but ~½ the cost-efficiency.
- **Data scale amplifies error cost:** CVQ shows a less-accurate model (Gemini 3 Pro) becomes far costlier at SF 1000 — a modest ~10% accuracy gap is critically amplified at scale (a failed query at SF 1000 is far more expensive than at SF 10).

## So what
For data-query agents on real warehouses, report a cost/efficiency metric (VES\*/VCES/CVQ) alongside execution accuracy — a "more accurate" model can be the wrong production choice once query cost, latency, and data scale are counted. Consider per-stage model assignment.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[data-query-agents|Data-query agents]]
- **Entities:** [[spider-benchmark]] · [[bird-benchmark]]
- **Raw:** alphaXiv full-text (id 2602.21480v4)

## Relationships
- evaluates [[data-query-agents]]
- part of [[agent-evaluation]]
- relates to [[bird-benchmark]], [[spider-benchmark]]
