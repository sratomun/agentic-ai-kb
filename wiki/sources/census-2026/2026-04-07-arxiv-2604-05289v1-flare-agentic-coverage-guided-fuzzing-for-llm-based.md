---
type: source
source_type: arxiv
title: "FLARE: Agentic Coverage-Guided Fuzzing for LLM-Based Multi-Agent Systems"
authors: Mingxuan Hui, Xinyue Li, Lu Wang, Chengcheng Wan et al.
url: https://arxiv.org/abs/2604.05289v1
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.SE
tags: [tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# FLARE: Agentic Coverage-Guided Fuzzing for LLM-Based Multi-Agent Systems

**arXiv:** [2604.05289v1](https://arxiv.org/abs/2604.05289v1) · 2026-04-07 · cs.SE
**Authors:** Mingxuan Hui, Xinyue Li, Lu Wang, Chengcheng Wan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-Agent LLM Systems (MAS) have been adopted to automate complex human workflows by breaking down tasks into subtasks. However, due to the non-deterministic behavior of LLM agents and the intricate interactions between agents, MAS applications frequently encounter failures, including infinite loops and failed tool invocations. Traditional software testing techniques are ineffective in detecting such failures due to the lack of LLM agent specification, the large behavioral space of MAS, and semantic-based correctness judgment. This paper presents FLARE, a novel testing framework tailored for MAS. FLARE takes the source code of MAS as input and extracts specifications and behavioral spaces from agent definitions. Based on these specifications, FLARE builds test oracles and conducts coverage-guided fuzzing to expose failures. It then analyzes execution logs to judge whether each test has passed and generates failure reports. Our evaluation on 16 diverse open-source applications demonstrates that FLARE achieves 96.9% inter-agent coverage and 91.1% intra-agent coverage, outperforming baselines by 9.5% and 1.0%. FLARE also uncovers 56 previously unknown failures unique to MAS.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.05289v1)
