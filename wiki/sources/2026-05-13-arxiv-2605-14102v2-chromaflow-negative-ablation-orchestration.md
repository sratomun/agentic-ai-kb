---
type: source
source_type: arxiv
title: "ChromaFlow: A Negative Ablation Study of Orchestration Overhead in Tool-Augmented Agent Evaluation"
authors: Tarun Mittal
url: https://arxiv.org/abs/2605.14102v2
date: 2026-05-13
ingested: 2026-06-21
depth: full-text
tags: [agent-evaluation, multi-agent-systems, arxiv]
---

# ChromaFlow: A Negative Ablation Study of Orchestration Overhead in Tool-Augmented Agent Evaluation

**Why it matters:** A rare negative result worth keeping: more aggressive orchestration did NOT improve GAIA performance and increased operational noise. Antidote to orchestration hype.

## Takeaways
- [[gaia-benchmark|GAIA]] L1: frozen baseline 29/53 (54.7%); expanded-orchestration recovery config dropped to 27/53 (50.9%) while increasing tracebacks, timeouts, tool failures, and cost.
- Central finding is a negative ablation — orchestration overhead can hurt, and small diagnostic gains are unstable across samples.
- Argues bounded planner escalation, deterministic extraction, evidence reconciliation, provider-health gates, and run gates should be first-order eval requirements.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[gaia-benchmark]]
- **Raw:** `raw/arxiv/2605.14102v2.md` · `raw/arxiv/2605.14102v2.fulltext.md`
