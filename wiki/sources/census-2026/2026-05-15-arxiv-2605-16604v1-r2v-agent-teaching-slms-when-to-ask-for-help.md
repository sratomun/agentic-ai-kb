---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "R2V Agent: Teaching SLMs When to Ask for Help"
authors: Raghu Vamshi Hemadri et al.
url: https://arxiv.org/abs/2605.16604v1
date: 2026-05-15
score: 6
primary: cs.LG
tags: [arxiv, auto-ingested, small-language-models, tool-use, distillation]
---

# R2V Agent: Teaching SLMs When to Ask for Help

**arXiv:** [2605.16604v1](https://arxiv.org/abs/2605.16604v1) · 2026-05-15 · cs.LG
**Authors:** Raghu Vamshi Hemadri et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Efficient agentic systems should incur expensive frontier-model costs only on decisions where a cheaper local model is likely to fail. Existing LLM cascades usually route whole queries before execution, but task difficulty shifts mid-trajectory - after flaky tool calls, truncated observations, or compounding local errors - making pre-execution routing brittle. We introduce \textbf{R2V-Agent}, a risk-calibrated SLM-LLM routing framework for interactive agents. R2V combines four components: a distilled small language model (SLM) policy, a stronger teacher LLM, a lightweight process verifier that scores candidate actions at each step, and a calibrated step-level router. The router is our central contribution: after the SLM is trained, it estimates residual failure risk at each step and escalates only when teacher intervention is warranted. To make the routing problem well-defined, we first train a stable local SLM using a standard offline pipeline: behavioral cloning (BC) on teacher trajectories, followed by verifier-guided Direct Preference Optimization (DPO) with consistency regularization. The router is then trained on this fixed policy's residual failures using Brier-calibrated probability estimation and a Conditional Value-at-Risk (CVaR)-constrained objective that penalizes worst-case failures across perturbation seeds. Across HumanEval+, TextWorld, and TerminalBench with four SLM backbones, R2V improves the reliability-cost frontier: it achieves $94.3\%$ HumanEval+ success with $0.60\%$ LLM escalation, recovers TextWorld from $64.6\%$ SLM-only success to $98.2\%$ at $41.7\%$ escalation, and reaches $93.3\%$ TerminalBench success at $33.9\%$ LLM calls, roughly half the heuristic-router cost.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[tool-use]] · [[distillation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.16604v1)
