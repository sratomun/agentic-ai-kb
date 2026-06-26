---
type: source
source_type: arxiv
title: "Enhancing LLM Medical Coding with Structured External Knowledge"
authors: Yidong Gan, David D. Nguyen, Yang Lin, Peter Zhong et al.
url: https://arxiv.org/abs/2605.27377v2
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 4
primary: cs.CL
tags: [clinical-agents, knowledge-graph, agentic-rag, arxiv, auto-ingested]
---

# Enhancing LLM Medical Coding with Structured External Knowledge

**arXiv:** [2605.27377v2](https://arxiv.org/abs/2605.27377v2) · 2026-04-09 · cs.CL
**Authors:** Yidong Gan, David D. Nguyen, Yang Lin, Peter Zhong et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Accurate medical coding requires consulting authoritative resources such as the ICD tabular list and coding guidelines. Existing LLM-based automated methods largely rely on LLMs' internal knowledge, which is prone to hallucination and cannot keep pace with guideline updates. We introduce RAG-Coding, an agentic, training-free method that augments LLMs with structured external knowledge: the tabular list is encoded as a knowledge graph capturing hierarchical and instructional code relationships, and the guidelines are distilled into concise, code-specific summaries rather than retrieved as raw text. To enable our study, we also introduce MDACE-2025, expert re-annotations of the MDACE dataset under the 2025 ICD-10-CM/PCS guidelines, adding code sequencing and justification comments. On MDACE, RAG-Coding outperforms the best LLM-based baseline by 3--13\% in micro-F1 across five LLM backbones, and achieves comparable micro- and macro-F1 to the supervised state-of-the-art, with higher recall ($+$11\%) at the cost of precision ($-$6\%). On MDACE-2025, RAG-Coding outperforms all baselines, demonstrating effective generalisation to updated guidelines. Ablations confirm stepwise gains, highlighting the importance of integrating structured external knowledge for LLM-based medical coding.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agentic-rag|Agentic RAG]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.27377v2)
