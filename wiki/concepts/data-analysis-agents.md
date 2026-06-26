---
type: concept
tags: [agents, data-analysis, insights, rca, evaluation]
created: 2026-06-22
updated: 2026-06-22
source_count: 2
---

# Data-analysis & insight agents

*Agents that go beyond querying data to interpret it — generating insights, summarizing findings, and doing root-cause analysis.*

## What it is
Agents whose job is the *conclusion*, not the query: turning rows into a correct, non-trivial, faithful claim. Distinct from [[data-query-agents|text-to-SQL agents]] — the hard part isn't fetching the data, it's reasoning over it without fabricating or mistaking correlation for cause. Root-cause analysis (RCA) is the demanding sub-case.

## Why it matters
This is where "agent that touches our data" becomes genuinely useful *or* genuinely dangerous — a confidently wrong insight is worse than no insight. It's also where evaluation gets subtle (the answer can be right for the wrong reason), so it's a proving ground for the [[agent-evaluation]] and [[agent-reliability]] disciplines on real enterprise output.

## What the evidence shows
**2026 developments — evaluation is the substance.** The work here is mostly about *measuring* analysis quality, decomposed into stages:
- **RCA eval = trajectory, not just the answer.** Cloud-OpsBench (452 faults / 40 root-cause types) scores process metrics (A@1/A@3 + trajectory alignment + ZTDR) and exposes the gap between explicit faults (A@1 > 0.65) and implicit ones (< 0.36) → [[2026-02-28-arxiv-2603-00468v1-cloud-opsbench-agentic-rca]] (cf. [[cloud-opsbench]]).
- **A shipped insight agent** is scored on relevance/correctness/completeness *and* tail latency (89.5% question-level accuracy, P90 13.56s) → [[2026-01-27-arxiv-2601-20048v2-insight-agents-data-insights]] (cf. [[insight-agents]]).

The eval decomposition to carry forward: computation correctness (numbers tie out — verify deterministically) → insight correctness (claim supported by data) → for RCA, root-cause precision/recall + causal validity → narrative faithfulness (no fabricated stats) → production latency. The failure mode to watch: right query, wrong interpretation.

## Relationships
- builds on [[data-query-agents]]
- evaluated under [[agent-evaluation]]
- relates to [[agent-reliability]], [[agentic-rag]]
- exemplars: [[cloud-opsbench]], [[insight-agents]]

## Key papers (citation-ranked)
<!-- Auto-maintained by kg-curator enrich. Citations from census/source-note frontmatter. -->
- **21** · 2.0/mo · [[2025-08-07-arxiv-2508-05002-agenticdata-heterogeneous-data|AgenticData: An Agentic Data Analytics System for Heterogeneous Da…]]
- **0** · [[2026-02-28-arxiv-2603-00468v1-cloud-opsbench-agentic-rca|Cloud-OpsBench: A Reproducible Benchmark for Agentic Root Cause An…]]
- **0** · [[2026-01-27-arxiv-2601-20048v2-insight-agents-data-insights|Insight Agents: An LLM-Based Multi-Agent System for Data Insights]]
