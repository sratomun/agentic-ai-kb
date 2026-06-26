---
type: source
source_type: arxiv
title: "Beyond the All-in-One Agent: Benchmarking Role-Specialized Multi-Agent Collaboration in Enterprise Workflows"
authors: Tao Yu, Hao Wang, Changyu Li, Shenghua Chai et al.
url: https://arxiv.org/abs/2605.08761v1
date: 2026-05-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MA
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Beyond the All-in-One Agent: Benchmarking Role-Specialized Multi-Agent Collaboration in Enterprise Workflows

**arXiv:** [2605.08761v1](https://arxiv.org/abs/2605.08761v1) · 2026-05-09 · cs.MA
**Authors:** Tao Yu, Hao Wang, Changyu Li, Shenghua Chai et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM) agents are increasingly expected to operate in enterprise environments, where work is distributed across specialized roles, permission-controlled systems, and cross-departmental procedures. However, existing enterprise benchmarks largely evaluate single agents with broad tool access, while existing multi-agent benchmarks rarely capture realistic enterprise constraints such as role specialization, access control, stateful business systems, and policy-based approvals. We introduce \textsc{EntCollabBench}, a benchmark for evaluating enterprise multi-agent collaboration. \textsc{EntCollabBench} simulates a permission-isolated organization with 11 role-specialized agents across six departments and contains two evaluation subsets: a Workflow subset, where agents collaboratively modify enterprise system states, and an Approval subset, where agents make policy-grounded decisions. Evaluation is based on execution traces, database state verification, and deterministic policy adjudication rather than natural-language response judging. Experiments with representative LLM agents show that current models still struggle with end-to-end enterprise collaboration, especially in delegation, context transfer, parameter grounding, workflow closure, and decision commitment. \textsc{EntCollabBench} provides a reproducible testbed for measuring and improving agent systems intended for realistic organizational environments.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.08761v1)
