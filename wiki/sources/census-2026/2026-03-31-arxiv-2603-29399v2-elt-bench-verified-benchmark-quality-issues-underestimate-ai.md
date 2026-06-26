---
type: source
source_type: arxiv
title: "ELT-Bench-Verified: Benchmark Quality Issues Underestimate AI Agent Capabilities"
authors: Christopher Zanoli, Andrea Giovannini, Tengjun Jin, Ana Klimovic et al.
url: https://arxiv.org/abs/2603.29399v2
date: 2026-03-31
ingested: 2026-06-21
depth: abstract
auto: true
score: 8
primary: cs.AI
tags: [data-query-agents, agent-reliability, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# ELT-Bench-Verified: Benchmark Quality Issues Underestimate AI Agent Capabilities

**arXiv:** [2603.29399v2](https://arxiv.org/abs/2603.29399v2) · 2026-03-31 · cs.AI
**Authors:** Christopher Zanoli, Andrea Giovannini, Tengjun Jin, Ana Klimovic et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Constructing Extract-Load-Transform (ELT) pipelines is a labor-intensive data engineering task and a high-impact target for AI automation. On ELT-Bench, the first benchmark for end-to-end ELT pipeline construction, AI agents initially showed low success rates, suggesting they lacked practical utility. We revisit these results and identify two factors causing a substantial underestimation of agent capabilities. First, re-evaluating ELT-Bench with upgraded large language models reveals that the extraction and loading stage is largely solved, while transformation performance improves significantly. Second, we develop an Auditor-Corrector methodology that combines scalable LLM-driven root-cause analysis with rigorous human validation (inter-annotator agreement Fleiss' kappa = 0.85) to audit benchmark quality. Applying this to ELT-Bench uncovers that most failed transformation tasks contain benchmark-attributable errors -- including rigid evaluation scripts, ambiguous specifications, and incorrect ground truth -- that penalize correct agent outputs. Based on these findings, we construct ELT-Bench-Verified, a revised benchmark with refined evaluation logic and corrected ground truth. Re-evaluating on this version yields significant improvement attributable entirely to benchmark correction. Our results show that both rapid model improvement and benchmark quality issues contributed to underestimating agent capabilities. More broadly, our findings echo observations of pervasive annotation errors in text-to-SQL benchmarks, suggesting quality issues are systemic in data engineering evaluation. Systematic quality auditing should be standard practice for complex agentic tasks. We release ELT-Bench-Verified to provide a more reliable foundation for progress in AI-driven data engineering automation.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.29399v2)
