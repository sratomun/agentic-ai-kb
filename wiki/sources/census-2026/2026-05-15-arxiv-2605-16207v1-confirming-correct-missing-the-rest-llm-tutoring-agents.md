---
type: source
source_type: arxiv
title: "Confirming Correct, Missing the Rest: LLM Tutoring Agents Struggle Where Feedback Matters Most"
authors: Tahreem Yasir, Wenbo Li, Sam Gilson, Sutapa Dey Tithi et al.
url: https://arxiv.org/abs/2605.16207v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.AI
tags: [clinical-agents, knowledge-graph, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# Confirming Correct, Missing the Rest: LLM Tutoring Agents Struggle Where Feedback Matters Most

**arXiv:** [2605.16207v1](https://arxiv.org/abs/2605.16207v1) · 2026-05-15 · cs.AI
**Authors:** Tahreem Yasir, Wenbo Li, Sam Gilson, Sutapa Dey Tithi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Effective tutoring requires distinguishing optimal, valid but suboptimal, and incorrect student solutions, a distinction central to intelligent tutoring systems (ITS) but untested for LLM-based tutors. As LLMs are increasingly explored as conversational complements to ITS, evaluating their diagnostic precision is essential. We present a benchmark of seven LLM feedback agents in propositional logic using knowledge-graph-derived ground truth across 10,836 solution--feedback pairs and three feedback conditions. Models achieved near-ceiling performance on optimal steps but systematically over-rejected valid but suboptimal reasoning and over-validated incorrect solutions, precisely where adaptive tutoring matters most. These failures persisted across models regardless of solution context, suggesting architectural rather than informational limits. Moreover, accurate diagnosis did not reliably produce pedagogically actionable feedback, revealing a gap between diagnostic judgment and instructional effectiveness. Our findings suggest that LLMs are better suited for hybrid architectures where KG-grounded models handle diagnosis while LLMs support open-ended scaffolding and dialogue.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16207v1)
