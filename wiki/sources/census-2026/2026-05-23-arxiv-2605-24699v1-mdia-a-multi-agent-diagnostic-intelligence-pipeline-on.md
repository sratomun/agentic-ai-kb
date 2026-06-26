---
type: source
source_type: arxiv
title: "MDIA: A Multi-Agent Diagnostic Intelligence Pipeline on HealthBench Professional"
authors: Roberto Cruz, David Rey-Blanco
url: https://arxiv.org/abs/2605.24699v1
date: 2026-05-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [clinical-agents, agent-reliability, agent-security, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# MDIA: A Multi-Agent Diagnostic Intelligence Pipeline on HealthBench Professional

**arXiv:** [2605.24699v1](https://arxiv.org/abs/2605.24699v1) · 2026-05-23 · cs.AI
**Authors:** Roberto Cruz, David Rey-Blanco

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Most reported gains on agentic-LLM clinical benchmarks are often attributed to prompt engineering, yet our results suggest that larger improvements can come from architectural and engine-level design. We present MDIA, a Multi-agent Diagnostic Intelligence Agent implemented as a 7-node specialty-routed clinical reasoning graph, on the full HealthBench Professional benchmark (n = 525), on a non-fine-tuned LLM. MDIA achieves 0.6272 under OpenAI's GPT-5.4-2026-03-05, which is +3.72 pp above the performance of OpenAI's ChatGPT for Clinicians. The experimental work shows that performance lift is attributable to system architecture: specialty routing, multi-turn context preservation, drug-state safety gating, site-filtered search, length-aware synthesis, and engine-level reliability. These findings support the view that agentic clinical benchmark performance is shaped both by the underlying foundation model and the orchestration architecture. Nevertheless, we also noticed notable differences when using other models as a grader; in particular, when using Gemini 2.5 Pro, MDIA scored 0.6585, which suggests that the choice of grader is a source of variability. Robust evaluation of LLMs would therefore require assessment across several independent grader models.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.24699v1)
