---
type: source
source_type: arxiv
title: "Agentic AI-based Framework for Mitigating Premature Diagnostic Handoff and Silent Hallucination in Healthcare Applications"
authors: Divyansh Srivastava, Shreya Ghosh, Anshul Verma, Rajkumar Buyya
url: https://arxiv.org/abs/2606.18068v1
date: 2026-06-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [clinical-agents, agent-security, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# Agentic AI-based Framework for Mitigating Premature Diagnostic Handoff and Silent Hallucination in Healthcare Applications

**arXiv:** [2606.18068v1](https://arxiv.org/abs/2606.18068v1) · 2026-06-16 · cs.AI
**Authors:** Divyansh Srivastava, Shreya Ghosh, Anshul Verma, Rajkumar Buyya

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Large Language Models (LLMs) and multi-agent systems have driven the rise of Agentic AI, showing promise for medical reasoning. However, open-ended conversational agents remain prone to two critical failure modes: premature diagnostic handoff and silent clinical hallucinations that may go undetected before reaching the patient. In this work, we propose a multi-agent framework that addresses both issues by replacing ``LLM-as-a-judge'' routing with deterministic orchestration constraints. The framework incorporates two safety mechanisms. First, a neuro-symbolic state-tracking gate enforces completeness of the OLDCARTS clinical protocol (Onset, Location, Duration, Character, Aggravating/Alleviating factors, Radiation, Timing, and Severity) by blocking diagnostic transitions until all required dimensions are collected. Second, an epistemic uncertainty quantification (UQ) gate computes semantic entropy (H) across K=5 independent diagnostic samples to identify and intercept divergent outputs before delivery. We evaluate the system using simulated patient agents powered by the llama-3.1-70b-instruct model on 150 test cases. The full architecture achieves 49.3% diagnostic precision, representing an absolute improvement of 11.3 percentage points over an unconstrained baseline. Additionally, we observe a statistically significant negative correlation (r = -0.181, p < 0.05) between OLDCARTS completeness (σ) and semantic entropy (H), suggesting that structured information gathering is associated with reduced diagnostic uncertainty.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[llama]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.18068v1)
