---
type: source
source_type: arxiv
title: "When Agents Overtrust Environmental Evidence: An Extensible Agentic Framework for Benchmarking Evidence-Grounding Defects in LLM Agents"
authors: Strick Sheng, Ziyue Wang, Liyi Zhou
url: https://arxiv.org/abs/2605.08828v2
date: 2026-05-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.AI
tags: [agent-reliability, agent-security, agent-memory, tool-use, agent-evaluation, arxiv, auto-ingested]
---

# When Agents Overtrust Environmental Evidence: An Extensible Agentic Framework for Benchmarking Evidence-Grounding Defects in LLM Agents

**arXiv:** [2605.08828v2](https://arxiv.org/abs/2605.08828v2) · 2026-05-09 · cs.AI
**Authors:** Strick Sheng, Ziyue Wang, Liyi Zhou

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model agents increasingly operate through environment-facing scaffolds that expose files, web pages, APIs, and logs. These observations influence tool use, state tracking, and action sequencing, yet their reliability and authority are often uncertain. Environmental grounding is therefore a systems-level problem involving context admission, evidence provenance, freshness checking, verification policy, action gating, and model reasoning. Existing agent benchmarks mainly evaluate task capability or specific attacks such as prompt injection and memory poisoning, but they under-specify a fundamental reliability question: whether agents remain grounded in the true environment state when observations are stale, incorrect, or malicious. We introduce EnvTrustBench, an agentic framework for benchmarking this failure mode. We define an evidence-grounding defect (EGD) as a behavioral failure in which an agent treats an environment-facing claim as sufficient evidence for action without resolving it against available current evidence, leading to a task-incorrect false path under the true environment state. Given a task scenario, EnvTrustBench generates the workspace, environment, agent-facing objective, and validation oracle, executes the evaluated agent, records its action-observation trajectory and final state, and applies the oracle to produce a verdict. Using 6 LLM backbones and 5 widely used scaffolds, we evaluate 55 generated cases across 11 task scenarios, with each scenario expanded through five feedback-guided generation iterations. Results show that EGDs consistently emerge across operational workflows, highlighting environmental grounding as a core agent reliability problem with important security implications.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.08828v2)
