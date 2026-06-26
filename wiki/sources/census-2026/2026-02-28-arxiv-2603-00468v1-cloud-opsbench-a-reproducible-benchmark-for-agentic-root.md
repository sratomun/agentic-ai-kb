---
type: source
source_type: arxiv
title: "Cloud-OpsBench: A Reproducible Benchmark for Agentic Root Cause Analysis in Cloud Systems"
authors: Yilun Wang, Guangba Yu, Haiyu Huang, Zirui Wang et al.
url: https://arxiv.org/abs/2603.00468v1
date: 2026-02-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.SE
tags: [clinical-agents, agent-reliability, agentic-rl, agent-protocols, multi-agent-systems, arxiv, auto-ingested]
---

# Cloud-OpsBench: A Reproducible Benchmark for Agentic Root Cause Analysis in Cloud Systems

**arXiv:** [2603.00468v1](https://arxiv.org/abs/2603.00468v1) · 2026-02-28 · cs.SE
**Authors:** Yilun Wang, Guangba Yu, Haiyu Huang, Zirui Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The transition to agentic Root Cause Analysis (RCA) necessitates benchmarks that evaluate active reasoning rather than passive classification. However, current frameworks fail to reconcile ecological validity with reproducibility. We introduce Cloud-OpsBench, a large-scale benchmark that employs a State Snapshot Paradigm to construct a deterministic digital twin of the cloud, featuring 452 distinct fault cases across 40 root cause types spanning the full Kubernetes stack. Crucially, Cloud-OpsBench serves as an enabling infrastructure for next-generation SRE research: (1) As a Data Engine, it harvests high-quality reasoning trajectories to bootstrap Supervised Fine-Tuning (SFT) for Small Language Models; (2) As an Reinforcement Learning (RL) environment, it transforms high-risk operations into a safe low-latency sandbox for training policy optimization agents; and (3) As a Diagnostic Standard, its process-centric protocol uncovers architectural bottlenecks guiding the design of robust specialized multi-agent system for RCA.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-protocols|Agent protocols]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00468v1)
