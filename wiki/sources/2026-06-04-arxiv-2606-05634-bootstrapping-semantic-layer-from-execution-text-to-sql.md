---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Bootstrapping Semantic Layer from Execution for Text-to-SQL"
authors: Youngwon Lee, Jaejin Kim, Seung-won Hwang (Seoul National University)
url: https://arxiv.org/abs/2606.05634
date: 2026-06-04
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-grounding, data-query-agents, agentic-rag, knowledge-graph]
---

# Bootstrapping Semantic Layer from Execution for Text-to-SQL

**arXiv [2606.05634](https://arxiv.org/abs/2606.05634)** · 2026-06-04 · Seoul National University

**Significance.** Where the semantic layer doesn't exist yet, *build it from execution*. GATE keeps multiple grounding hypotheses open, runs the grounded parts, and keeps only the interpretation the data supports — accumulating a reusable semantic layer. The "bootstrap the grounding" anchor for [[intent-grounding]].

## Abstract
Real-world text-to-SQL is under-specified until user phrases are grounded in how the database stores values. Prior work grounds "too early" (before inference, during execution, or during decomposition). GATE (Grounding After Test from Execution) reframes the query as a partially grounded plan and grounds each hypothesis only when execution observations support it, caching verified groundings as reusable memory.

## From the paper (full-text, via subagent)
**Contribution / method.** **GATE** models an under-specified query as a CTE-like plan where some operators are ungrounded; it keeps multiple grounding hypotheses **open**, executes already-grounded parts to get observations, then grounds **only the hypothesis the observation supports**. Verified groundings become **memory entries** (executable query body + evidence summary) — an "execution-grounded semantic layer" that accumulates. Components: plan evaluation, plan selection, evidence summarization, grounding-update reuse.
**Results.** With GPT-5.4-mini, GATE hits **55.2% on RealEHR** (vs ReAct 42.9, ReDel 44.8, ReFoRCE 48.6), **34.4% EX on EHRSQL**, **45.1% on LS-Hard**. Ablation (RealEHR): removing plan evaluation costs **-10.5pp** (largest), evidence summarization **-8.4pp**. Cost: 55.2% at 36.0 LLM calls/query beats ReAct×6 (51.1% at 39.1) — more accurate, cheaper. Memory: 912 grounding updates, **97.8% reused** across plans, **99.5% update accuracy**, contradiction rate 0.011%.
**Takeaway.** Execution is a *bootstrapping* signal, not just SQL validation: keep grounding ambiguous intent open until the data disambiguates it, then cache it. Fills the schema gaps that under-documented expert domains (clinical EHR) leave.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[data-query-agents]] · [[agentic-rag]] · [[knowledge-graph]]
- **Entities:** [[metrics-layer]]
- **Raw:** full-text (alphaXiv, read via subagent) 2026-06-23
