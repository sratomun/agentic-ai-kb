---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Beyond Text-to-SQL: An Agentic LLM System for Governed Enterprise Analytics APIs"
authors: Gundeep Singh et al. (Dialpad)
url: https://arxiv.org/abs/2605.21027
date: 2026-05-20
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-grounding, intent-understanding, data-query-agents, knowledge-graph]
---

# Beyond Text-to-SQL: An Agentic LLM System for Governed Enterprise Analytics APIs

**arXiv [2605.21027](https://arxiv.org/abs/2605.21027)** · 2026-05-20 · Dialpad

**Significance.** The cleanest production statement of the semantic-layer thesis: don't let the LLM write SQL — make it a *planner over governed analytics APIs* (the semantic layer), where metric definitions, permissions, and audit live outside the model. The keystone for [[intent-grounding]] and the closest paper to the exec's own semantic-layer vault work.

## Abstract
Analytic Agent translates natural-language analytics intents into secure interactions with enterprise analytics APIs rather than raw databases. It combines agentic orchestration, target resolution, secure API execution, and policy-aware visualization, and on 90 expert-curated enterprise use cases reaches 77.22% end-to-end accuracy and 96.67% query-execution success.

## From the paper (full-text)
**Contribution / method.** A four-subsystem agent over **governed APIs, not SQL**: (i) Orchestrator (Parse→Targets→Query→Viz→Done, ≤1 disambiguation question per flow); (ii) **Target grounding + permissions** — fuzzy-matches NL references ("Support team in Seattle") to concrete org entities filtered by the user's access rights, checking permission before proceeding; (iii) **Database querying over governed APIs** — selects endpoint, builds a schema-compliant payload, and delegates date handling to **deterministic functions, not the LLM**, to cut hallucination; (iv) Visualization as governed structured generation (charts respect the same permissions; sensitive fields masked). Evaluated on 90 expert-authored tasks (300 hours of curation), judged binary by GPT-5.2 and Claude-Opus-4.6.
**Results.** Gemini-2.5-Pro: **77.22% end-to-end accuracy, 96.67% execution success**; Gemini-2.5-Flash 71.67% / 94.44% (chosen for production on cost/latency); Flash-Lite collapses to ~16-17% E2E despite 44% executable — **structural validity is necessary but not sufficient** (endpoint, target, and temporal filtering can be subtly wrong). Caching field definitions cut latency **22%** (24.84s→19.31s) and input cost **64%**.
**Takeaway (the money quote).** "The LLM should not be treated as the repository of business logic; it should act as a planner over stable, structured interfaces owned by the platform. Authentication, metric definitions, audit logging, and rendering all remain outside the model, while the model handles intent interpretation and tool selection." That separation is the whole argument for grounding intent in a semantic layer.

## Graph
- **Concepts:** [[intent-grounding|Intent grounding]] · [[intent-understanding|Intent understanding]] · [[data-query-agents]] · [[knowledge-graph]]
- **Entities:** [[metrics-layer]] · [[tau-bench]]
- **Raw:** full-text report (alphaXiv) read 2026-06-23
