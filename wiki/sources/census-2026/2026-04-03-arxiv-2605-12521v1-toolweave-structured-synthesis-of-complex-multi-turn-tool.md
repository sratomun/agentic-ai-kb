---
type: source
source_type: arxiv
title: "ToolWeave: Structured Synthesis of Complex Multi-Turn Tool-Calling Dialogues"
authors: Dinesh Khandelwal, Gnana Prakash Punnavajhala, GPS Bhargav, Gaurav Pandey et al.
url: https://arxiv.org/abs/2605.12521v1
date: 2026-04-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CL
tags: [tool-use, agent-evaluation, arxiv, auto-ingested]
---

# ToolWeave: Structured Synthesis of Complex Multi-Turn Tool-Calling Dialogues

**arXiv:** [2605.12521v1](https://arxiv.org/abs/2605.12521v1) · 2026-04-03 · cs.CL
**Authors:** Dinesh Khandelwal, Gnana Prakash Punnavajhala, GPS Bhargav, Gaurav Pandey et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Multi-turn tool calling is essential for LLMs to function as autonomous agents, yet synthesizing the training data required for these capabilities remains a fundamental challenge. Existing synthetic data generation pipelines often produce unrealistic dialogues for two reasons: they chain tools that are only superficially compatible rather than aligned with meaningful user tasks, and they generate dialogues in one shot, which often introduces arguments that were neither provided by the user nor produced by prior tool calls. These issues also lead to a severe underrepresentation of multi-step tool interactions. We introduce ToolWeave, a structured framework for synthesizing realistic multi-turn tool-calling dialogues. ToolWeave support realistic multi-step workflows (or tool sequences) by constructing tools with built-in dependencies and filters the workflows based on alignment with user goals. It reduces parameter hallucination by using a fine-grained planning stage that explicitly tracks parameter provenance. As a result, ToolWeave-generated synthetic dialogues contain more multi-step tool interactions (45%) and fewer hallucinations in parameters and tool names. Consequently, LLMs fine-tuned on ToolWeave consistently outperform those fine-tuned on prior datasets across three public benchmarks. Notably, Llama-3.1-70B fine-tuned on ToolWeave achieves 39.75% on BFCL-V3 multi-turn, compared to 23.50% when fine-tuned on SOTA ToolFlow data.

## Graph
- **Concepts:** [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[llama]] · [[bfcl]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12521v1)
