---
type: source
source_type: arxiv
title: "GUIDE: Interpretable GUI Agent Evaluation via Hierarchical Diagnosis"
authors: Yuwen Zhai, Runze Li, Liang Wang, Nian Shi et al.
url: https://arxiv.org/abs/2604.04399v1
date: 2026-04-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 12
primary: cs.AI
tags: [recommendation-agents, clinical-agents, computer-use-agents, agent-reliability, agent-memory, arxiv, auto-ingested]
---

# GUIDE: Interpretable GUI Agent Evaluation via Hierarchical Diagnosis

**arXiv:** [2604.04399v1](https://arxiv.org/abs/2604.04399v1) · 2026-04-06 · cs.AI
**Authors:** Yuwen Zhai, Runze Li, Liang Wang, Nian Shi et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Evaluating GUI agents presents a distinct challenge: trajectories are long, visually grounded, and open-ended, yet evaluation must be both accurate and interpretable. Existing approaches typically apply a single holistic judgment over the entire action-observation sequence-a strategy that proves unreliable on long-horizon tasks and yields binary verdicts offering no insight into where or why an agent fails. This opacity limits the utility of evaluation as a diagnostic tool for agent development. We introduce GUIDE (GUI Understanding and Interpretable Diagnostic Evaluation), a framework that decomposes trajectory assessment into three sequential stages mirroring the compositional structure of GUI tasks. Trajectory Segmentation partitions the full trace into semantically coherent subtask units. Subtask Diagnosis evaluates each unit in context, assigning a completion verdict and generating a structured error analysis with corrective recommendations. Overall Summary aggregates per-subtask diagnoses into a task-level judgment. By operating on bounded subtask segments rather than full trajectories, GUIDE mitigates the context overload that degrades existing evaluators as task complexity grows. We validate GUIDE on three benchmarks: an industrial e-commerce dataset of 932 trajectories, AGENTREWARDBENCH spanning five web agent tasks with 1302 trajectories, and AndroidBench for mobile device control. Across all settings, GUIDE substantially outperforms existing evaluators-achieving up to 5.35 percentage points higher accuracy than the strongest baseline-while producing structured diagnostic reports that directly inform agent improvement.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[clinical-agents|Clinical agents]] · [[computer-use-agents|Computer-use agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.04399v1)
