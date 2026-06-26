---
type: source
source_type: arxiv
title: "When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems"
authors: Zehao Wang, Shilong Jin, Zhao Cao, Lanjun Wang
url: https://arxiv.org/abs/2605.23414v1
date: 2026-05-22
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.AI
tags: [multi-agent-systems, arxiv, auto-ingested]
---

# When Planning Fails Despite Correct Execution: On Epistemic Calibration for LLM-Based Multi-Agent Systems

**arXiv:** [2605.23414v1](https://arxiv.org/abs/2605.23414v1) · 2026-05-22 · cs.AI
**Authors:** Zehao Wang, Shilong Jin, Zhao Cao, Lanjun Wang

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
LLM-based multi-agent systems can fail even when planned actions are executed correctly because agents may misjudge their knowledge when evaluating plan feasibility, a phenomenon we term epistemic miscalibration in planning. Unlike execution errors, epistemic miscalibration is latent during planning, as generated plans can remain self-consistent and executable without observable errors; the miscalibration is also dynamic, as new information can alter feasibility assessments, potentially obscuring past miscalibration signals and causing them to recur over time. To address this, we propose the Epistemic Planning Calibration Agentic Workflow (EPC-AW), which assesses whether plans remain supported under varying information conditions rather than directly verifying feasibility. EPC-AW employs Information-consistency-based Plan Selection, selecting plans whose evaluations are stable across agents, together with Consistency-guided Epistemic State Refinement to adapt calibration over time by leveraging past discrepancies to guide future planning. Experiments show that EPC-AW improves system-level success by an average of 9.75%.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.23414v1)
