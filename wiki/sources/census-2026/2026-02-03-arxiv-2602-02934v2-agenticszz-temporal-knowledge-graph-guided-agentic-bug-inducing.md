---
type: source
source_type: arxiv
title: "AgenticSZZ: Temporal Knowledge Graph-Guided Agentic Bug-Inducing Commit Identification"
authors: Yu Shi, Hao Li, Bram Adams, Ahmed E. Hassan
url: https://arxiv.org/abs/2602.02934v2
date: 2026-02-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.SE
tags: [coding-agents, embodied-agents, knowledge-graph, arxiv, auto-ingested]
---

# AgenticSZZ: Temporal Knowledge Graph-Guided Agentic Bug-Inducing Commit Identification

**arXiv:** [2602.02934v2](https://arxiv.org/abs/2602.02934v2) · 2026-02-03 · cs.SE
**Authors:** Yu Shi, Hao Li, Bram Adams, Ahmed E. Hassan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Identifying Bug-Inducing Commits (BICs) is fundamental for understanding software defects and enabling downstream tasks such as defect prediction and automated program repair. Yet existing SZZ-based approaches rely on git blame, restricting the search space to commits that directly modified the fixed lines. Our preliminary study on 2,102 validated bug-fixing commits reveals this limitation is significant: 28% of BICs require traversing commit history beyond blame results and 14% are blameless. We present AgenticSZZ, the first approach to apply Temporal Knowledge Graphs (TKGs) to software evolution analysis. AgenticSZZ reframes BIC identification from ranking blame commits into a graph search problem, where temporal ordering is fundamental to causal reasoning about bug introduction. The approach operates in two phases: (1) constructing a TKG that encodes commits with temporal and structural relationships, expanding the search space by traversing file history backward from blame commits and the bug-fixing commit; and (2) leveraging an LLM agent to navigate the graph using specialized tools for candidate exploration and causal analysis. Evaluation on three datasets shows that AgenticSZZ achieves F1-scores of 0.47 to 0.79, with statistically significant F1 improvements over state-of-the-art by up to 34%. Ablation confirms that both components and context expansion each contribute: the TKG and agent form an exploration-exploitation synergy, while context expansion unlocks ancestor BIC discovery, yielding 60 additional true positives. A sensitivity analysis across five open-weight LLMs reveals that effective TKG navigation requires sufficiently capable models, and that the TKG architecture amplifies stronger LLMs, widening the advantage. By transforming BIC identification into graph search, we open a new direction for temporal and causal reasoning in software evolution analysis.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[embodied-agents|Embodied agents]] · [[knowledge-graph|Knowledge graphs]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.02934v2)
