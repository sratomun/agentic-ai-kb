---
type: source
source_type: arxiv
title: "APEX-SQL: Talking to the data via Agentic Exploration for Text-to-SQL"
authors: Bowen Cao, Weibin Liao, Yushi Sun, Dong Fang et al.
url: https://arxiv.org/abs/2602.16720v2
date: 2026-02-11
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.DB
tags: [data-query-agents, science-agents, agent-evaluation, arxiv, auto-ingested]
---

# APEX-SQL: Talking to the data via Agentic Exploration for Text-to-SQL

**arXiv:** [2602.16720v2](https://arxiv.org/abs/2602.16720v2) · 2026-02-11 · cs.DB
**Authors:** Bowen Cao, Weibin Liao, Yushi Sun, Dong Fang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text-to-SQL systems powered by Large Language Models have excelled on academic benchmarks but struggle in complex enterprise environments. The primary limitation lies in their reliance on static schema representations, which fails to resolve semantic ambiguity and scale effectively to large, complex databases. To address this, we propose APEX-SQL, an Agentic Text-to-SQL Framework that shifts the paradigm from passive translation to agentic exploration. Our framework employs a hypothesis-verification loop to ground model reasoning in real data. In the schema linking phase, we use logical planning to verbalize hypotheses, dual-pathway pruning to reduce the search space, and parallel data profiling to validate column roles against real data, followed by global synthesis to ensure topological connectivity. For SQL generation, we introduce a deterministic mechanism to retrieve exploration directives, allowing the agent to effectively explore data distributions, refine hypotheses, and generate semantically accurate SQLs. Experiments on BIRD (70.65% execution accuracy) and Spider 2.0-Snow (51.01% execution accuracy) demonstrate that APEX-SQL outperforms competitive baselines with reduced token consumption. Further analysis reveals that agentic exploration acts as a performance multiplier, unlocking the latent reasoning potential of foundation models in enterprise settings. Ablation studies confirm the critical contributions of each component in ensuring robust and accurate data analysis. Our code is released at https://github.com/Tencent/APEX-SQL-Project.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[science-agents|Science agents]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[bird-benchmark]] · [[spider-benchmark]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.16720v2)
