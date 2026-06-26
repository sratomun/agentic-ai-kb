---
type: source
source_type: arxiv
title: "Benchmarking Text-to-Python against Text-to-SQL: The Impact of Explicit Logic and Ambiguity"
authors: Hangle Hu, Chenyu Hou, Bin Cao (Zhejiang Univ. of Technology), Ruizhe Li (Univ. of Aberdeen)
url: https://arxiv.org/abs/2601.15728v2
date: 2026-01-22
ingested: 2026-06-22
depth: full-text
tags: [agent-evaluation, data-query-agents, arxiv]
---

# Benchmarking Text-to-Python against Text-to-SQL

**Why it matters:** For text2query eval the headline isn't the model or the language — it's **domain grounding**. When ambiguous intent is resolved, Text-to-Python reaches parity with Text-to-SQL, so a lot of measured "code-gen weakness" is actually a grounding/ambiguity failure. Tells you to measure execution accuracy while explicitly isolating intent-grounding, and to clean annotation noise before trusting any score.

## What it is
**BIRD-Python:** the BIRD dev set (1,534 query–SQL pairs) refined to align execution semantics and reconstructed into Python/Pandas over file-based CSVs, enabling controlled SQL-vs-Python comparison. Evaluation uses an **LLM-based Execution Accuracy (EX)** semantic validator (human-audited on N=600) to avoid penalizing semantically-correct outputs with cosmetic differences (column order, types).

## Findings (verified)
- **Small models drop sharply on Python:** Qwen2.5-Coder-7B 52.93% (SQL) → 35.95% (Python); task-specialized AutoCoder/TableGPT2 collapse on Python (5.45%, 19.82%). The gap shrinks with larger/reasoning models — Qwen3-Max Python 63.43% ≈ SQL 63.10%.
- **Data quality matters:** on the verified set, Qwen3-Max +8.15% and DeepSeek-R1 +6.78% over the original BIRD dev — i.e. annotation noise was distorting scores.
- **Errors:** Filter-Condition errors dominate both paradigms (SQL 32.7%, Code 31.7%) — natural-language understanding is the shared bottleneck. Python shows far more Logic errors (17.5% vs SQL 0.3%) from needing explicit procedural steps.
- **Logic Completion Framework (LCF)** (inject ground-truth-derived clarifications): Qwen3-7B Code 53.19→71.19, SQL 61.22→71.38; Qwen3-32B reaches Code 72.49 ≈ SQL 72.75 (**parity**). Confirms the bottleneck is latent domain knowledge, not code generation.

## So what
Score text2query agents on **execution accuracy**, but read a low score carefully: it may be an ambiguity/grounding failure, not a generation failure. Clean reference annotations first (noise inflates/deflates by several points). Same lesson generalizes to any NL→executable-artifact task.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[data-query-agents|Data-query agents]]
- **Entities:** [[bird-python]] · [[bird-benchmark]]
- **Raw:** alphaXiv full-text (id 2601.15728v2)

## Relationships
- introduces [[bird-python]]
- evaluates [[data-query-agents]]
- part of [[agent-evaluation]]
