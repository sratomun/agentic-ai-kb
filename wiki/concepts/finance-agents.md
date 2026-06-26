---
type: concept
tags: [agents, finance, trading]
created: 2026-06-21
updated: 2026-06-22
census_count: 294
kind: domain
---

# Finance & trading agents

*Agents for financial analysis, trading, risk, and back-office finance — from quantitative strategy to document-centric automation.*

## What it is
LLM agents in finance workflows: market/document analysis, credit and fraud decisioning, trading strategy, and back-office automation — almost always in a setting where the output must be *explainable and reproducible*, not just accurate.

## Why it matters
A regulated, high-value vertical where the differentiator is **governed, auditable execution**, not raw autonomy — and it's adjacent to your own finance work. The pattern that wins here (typed plans, audit trails, deterministic checks) is the same one that earns trust in any regulated domain.

## What the evidence shows
**State of play.** The defining issue is **determinism, not capability**. The financial-AI survey reframes the problem as *reproducibility under regulation*: across tabular models, graph networks, and LLM agentic workflows, mechanical nondeterminism (batch-dependent divergence, trajectory drift) breaks auditability — and the answer is a layered evaluation framework that ties metrics to *audit readiness* rather than accuracy alone (→ [[2026-05-11-arxiv-2605-23955v2-survey-determinism-in-financial-ai]]). On the execution side, governed typed planning with compiled policy guardrails and full audit traces (POLARIS) is the back-office pattern — F1 0.81 on receipts, 0.95–1.00 anomaly-routing precision (→ [[polaris]]).
- _Honest note: large census cluster (~294), but agentic-specific deep work is thin and mostly 2026; treat the synthesis above as directional._

## Relationships
- governed by [[governance-gap]], [[agent-security]]
- determinism/auditability: see the financial-AI survey below
- exemplar: [[polaris]] (back-office finance)
- a form of [[agentic-ai]]

## Key papers
- [[2026-05-11-arxiv-2605-23955v2-survey-determinism-in-financial-ai|From Accuracy to Auditability: Determinism in Financial AI Systems (survey)]]
