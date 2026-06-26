---
type: source
source_type: arxiv
title: "Tool-Aware Planning in Contact Center AI: Evaluating LLMs through Lineage-Guided Query Decomposition"
authors: Varun Nathan, Shreyas Guha, Ayush Kumar
url: https://arxiv.org/abs/2602.14955v1
date: 2026-02-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.CL
tags: [data-query-agents, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Tool-Aware Planning in Contact Center AI: Evaluating LLMs through Lineage-Guided Query Decomposition

**arXiv:** [2602.14955v1](https://arxiv.org/abs/2602.14955v1) · 2026-02-16 · cs.CL
**Authors:** Varun Nathan, Shreyas Guha, Ayush Kumar

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
We present a domain-grounded framework and benchmark for tool-aware plan generation in contact centers, where answering a query for business insights, our target use case, requires decomposing it into executable steps over structured tools (Text2SQL (T2S)/Snowflake) and unstructured tools (RAG/transcripts) with explicit depends_on for parallelism. Our contributions are threefold: (i) a reference-based plan evaluation framework operating in two modes - a metric-wise evaluator spanning seven dimensions (e.g., tool-prompt alignment, query adherence) and a one-shot evaluator; (ii) a data curation methodology that iteratively refines plans via an evaluator->optimizer loop to produce high-quality plan lineages (ordered plan revisions) while reducing manual effort; and (iii) a large-scale study of 14 LLMs across sizes and families for their ability to decompose queries into step-by-step, executable, and tool-assigned plans, evaluated under prompts with and without lineage. Empirically, LLMs struggle on compound queries and on plans exceeding 4 steps (typically 5-15); the best total metric score reaches 84.8% (Claude-3-7-Sonnet), while the strongest one-shot match rate at the "A+" tier (Extremely Good, Very Good) is only 49.75% (o3-mini). Plan lineage yields mixed gains overall but benefits several top models and improves step executability for many. Our results highlight persistent gaps in tool-understanding, especially in tool-prompt alignment and tool-usage completeness, and show that shorter, simpler plans are markedly easier. The framework and findings provide a reproducible path for assessing and improving agentic planning with tools for answering data-analysis queries in contact-center settings.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.14955v1)
