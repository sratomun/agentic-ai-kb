---
type: source
source_type: arxiv
title: "FinToolBench: Evaluating LLM Agents for Real-World Financial Tool Use"
authors: Jiaxuan Lu, Kong Wang, Yemin Wang, Qingmei Tang et al.
url: https://arxiv.org/abs/2603.08262v1
date: 2026-03-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [finance-agents, tool-use, agent-evaluation, governance-gap, arxiv, auto-ingested]
---

# FinToolBench: Evaluating LLM Agents for Real-World Financial Tool Use

**arXiv:** [2603.08262v1](https://arxiv.org/abs/2603.08262v1) · 2026-03-09 · cs.AI
**Authors:** Jiaxuan Lu, Kong Wang, Yemin Wang, Qingmei Tang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The integration of Large Language Models (LLMs) into the financial domain is driving a paradigm shift from passive information retrieval to dynamic, agentic interaction. While general-purpose tool learning has witnessed a surge in benchmarks, the financial sector, characterized by high stakes, strict compliance, and rapid data volatility, remains critically underserved. Existing financial evaluations predominantly focus on static textual analysis or document-based QA, ignoring the complex reality of tool execution. Conversely, general tool benchmarks lack the domain-specific rigor required for finance, often relying on toy environments or a negligible number of financial APIs. To bridge this gap, we introduce FinToolBench, the first real-world, runnable benchmark dedicated to evaluating financial tool learning agents. Unlike prior works limited to a handful of mock tools, FinToolBench establishes a realistic ecosystem coupling 760 executable financial tools with 295 rigorous, tool-required queries. We propose a novel evaluation framework that goes beyond binary execution success, assessing agents on finance-critical dimensions: timeliness, intent type, and regulatory domain alignment. Furthermore, we present FATR, a finance-aware tool retrieval and reasoning baseline that enhances stability and compliance. By providing the first testbed for auditable, agentic financial execution, FinToolBench sets a new standard for trustworthy AI in finance. The tool manifest, execution environment, and evaluation code will be open-sourced to facilitate future research.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]] · [[governance-gap|Governance gap]]
- **Entities:** [[toolbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08262v1)
