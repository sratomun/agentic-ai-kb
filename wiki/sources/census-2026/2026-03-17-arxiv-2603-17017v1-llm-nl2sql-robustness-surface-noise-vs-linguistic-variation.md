---
type: source
source_type: arxiv
title: "LLM NL2SQL Robustness: Surface Noise vs. Linguistic Variation in Traditional and Agentic Settings"
authors: Lifu Tu, Rongguang Wang, Tao Sheng, Sujjith Ravi et al.
url: https://arxiv.org/abs/2603.17017v1
date: 2026-03-17
ingested: 2026-06-21
depth: abstract
auto: true
score: 9
primary: cs.CL
tags: [data-query-agents, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# LLM NL2SQL Robustness: Surface Noise vs. Linguistic Variation in Traditional and Agentic Settings

**arXiv:** [2603.17017v1](https://arxiv.org/abs/2603.17017v1) · 2026-03-17 · cs.CL
**Authors:** Lifu Tu, Rongguang Wang, Tao Sheng, Sujjith Ravi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Robustness evaluation for Natural Language to SQL (NL2SQL) systems is essential because real-world database environments are dynamic, noisy, and continuously evolving, whereas conventional benchmark evaluations typically assume static schemas and well-formed user inputs. In this work, we introduce a robustness evaluation benchmark containing approximately ten types of perturbations and conduct evaluations under both traditional and agentic settings. We assess multiple state-of-the-art large language models (LLMs), including Grok-4.1, Gemini-3-Pro, Claude-Opus-4.6, and GPT-5.2. Our results show that these models generally maintain strong performance under several perturbations; however, notable performance degradation is observed for surface-level noise (e.g., character-level corruption) and linguistic variation that preserves semantics while altering lexical or syntactic forms. Furthermore, we observe that surface-level noise causes larger performance drops in traditional pipelines, whereas linguistic variation presents greater challenges in agentic settings. These findings highlight the remaining challenges in achieving robust NL2SQL systems, particularly in handling linguistic variability.

## Graph
- **Concepts:** [[data-query-agents|Data-query agents]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[claude]] · [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.17017v1)
