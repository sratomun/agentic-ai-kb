---
type: source
source_type: arxiv
title: "Can LLMs Be CEOs? Benchmarking Strategic Resource Reallocation with Multi-Role Agent Simulation"
authors: Yuyang Dai, Xueqing Peng, Lingfei Qian, Zhuohan Xie
url: https://arxiv.org/abs/2606.17459v1
date: 2026-06-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.AI
tags: [recommendation-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Can LLMs Be CEOs? Benchmarking Strategic Resource Reallocation with Multi-Role Agent Simulation

**arXiv:** [2606.17459v1](https://arxiv.org/abs/2606.17459v1) · 2026-06-16 · cs.AI
**Authors:** Yuyang Dai, Xueqing Peng, Lingfei Qian, Zhuohan Xie

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Evaluating the decision-making capabilities of large language models (LLMs) is a growing research priority, yet existing benchmarks focus on isolated cognitive tasks such as reasoning, knowledge retrieval, and economic rationality in stylized settings. These evaluations overlook the defining challenge of real executive decision-making: integrating conflicting recommendations from specialized stakeholders under information asymmetry, organizational constraints, and temporal dependencies. We introduce \textsc{CEO-Bench}, a multi-agent benchmark that evaluates LLMs on CEO-level strategic resource reallocation -- the process of redirecting capital across business units in a multi-round, constraint-rich organizational environment. In \textsc{CEO-Bench}, LLM agents receive conflicting advice from four role-conditioned C-suite advisors (CFO, CTO, COO, CMO), each with private signals and distinct priorities, and must synthesize these into a concrete allocation plan evaluated along four dimensions: role integration, conditional boldness, history-sensitive judgment, and plan validity. Experiments across five frontier models on 13 scenarios reveal that all models achieve high structural validity but diverge sharply on strategic calibration -- the hardest capability layer. We identify systematic failure modes including single-advisor capture, conservative default under ambiguity, and historical amnesia, and uncover a structural integration-boldness tradeoff: models that engage more deeply with conflicting perspectives tend to produce less decisive action. These findings delineate the current capability boundary of LLMs as organizational decision-makers and inform the design of future AI-assisted executive systems.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.17459v1)
