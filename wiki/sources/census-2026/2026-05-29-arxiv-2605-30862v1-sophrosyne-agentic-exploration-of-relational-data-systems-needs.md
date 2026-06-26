---
type: source
source_type: arxiv
title: "Sophrosyne: Agentic Exploration of Relational Data Systems Needs Moderation"
authors: Madhav Jivrajani, Ramnatthan Alagappan, Aishwarya Ganesan
url: https://arxiv.org/abs/2605.30862v1
date: 2026-05-29
ingested: 2026-06-21
depth: abstract
auto: true
score: 7
primary: cs.DB
tags: [data-query-agents, tool-use, arxiv, auto-ingested]
---

# Sophrosyne: Agentic Exploration of Relational Data Systems Needs Moderation

**arXiv:** [2605.30862v1](https://arxiv.org/abs/2605.30862v1) · 2026-05-29 · cs.DB
**Authors:** Madhav Jivrajani, Ramnatthan Alagappan, Aishwarya Ganesan

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Text2SQL agents powered by LLMs translate natural language intent into SQL by exploring the data system through tool calls before formulating the query. However, to ensure secure and scoped access, data systems construct environments with explicit API surfaces. We study and categorize these APIs exposed today as either coarse-grained or fine-grained and posit that choosing between them presents a fundamental tradeoff between cost-efficient exploration and accurate SQL generation. Most data systems expose fine-grained APIs, but this inadvertently disadvantages agents: they over-explore, incorporating irrelevant schema elements into their query formulation and produce inaccurate results. We argue that curbing over-exploration is key to the effective use of these API surfaces, and propose Sophrosyne, a data system environment that augments API responses with directives that guide the agent's exploration process. Initial results show that directives reduce over-exploration by 4.6x and boost accuracy by up to 12.4% (approx. 4 percentage points).

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.30862v1)
