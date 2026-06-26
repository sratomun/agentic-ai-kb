---
type: source
source_type: arxiv
title: "ProcCtrlBench: Evaluating Process-Level Defects and Control Preservation in LLM Coding Agents"
authors: Jiawei He, Jie Jia, Chenbo Liu, Chaoyi Xue et al.
url: https://arxiv.org/abs/2605.20251v4
date: 2026-05-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 5
primary: cs.SE
tags: [coding-agents, computer-use-agents, knowledge-graph, agent-reliability, agent-evaluation, arxiv, auto-ingested]
---

# ProcCtrlBench: Evaluating Process-Level Defects and Control Preservation in LLM Coding Agents

**arXiv:** [2605.20251v4](https://arxiv.org/abs/2605.20251v4) · 2026-05-18 · cs.SE
**Authors:** Jiawei He, Jie Jia, Chenbo Liu, Chaoyi Xue et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Existing benchmarks for LLM coding agents primarily evaluate final outcomes. While useful for measuring overall capability, these metrics provide limited visibility and often miss defects that arise during execution. We present ProcCtrlBench, a benchmark for execution-process evaluation in LLM coding agents. ProcCtrlBench organizes recurrent execution defects into a reusable ontology covering 11 defect types in 4 categories, and evaluates agent trajectories through standardized process evidence rather than final outcomes alone. To support comparison across heterogeneous agents, ProcCtrlBench standardizes raw logs into a unified trajectory representation and reports calibrated scorecards over process-level findings. In addition, ProcCtrlBench uses control preservation as a way to quantify execution-process quality, capturing whether execution remains interpretable, interruptible, correctable, reversible, and able to hand back authority when needed. We evaluate ProcCtrlBench on 200 cases sampled from three benchmarks: AndroidBench, TerminalBench, and SWE-bench-Verified. Results show that ProcCtrlBench can be instantiated with useful reliability, provides more stable semantics than direct thresholding, and reveals meaningful differences in execution quality that are often overlooked by conventional outcome-based evaluation.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[computer-use-agents|Computer-use agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[swe-bench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.20251v4)
