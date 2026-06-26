---
type: source
source_type: arxiv
title: "A Trace-Based Assurance Framework for Agentic AI Orchestration: Contracts, Testing, and Governance"
authors: Ciprian Paduraru, Petru-Liviu Bouruc, Alin Stefanescu
url: https://arxiv.org/abs/2603.18096v1
date: 2026-03-18
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.MA
tags: [agent-reliability, agent-security, agent-memory, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# A Trace-Based Assurance Framework for Agentic AI Orchestration: Contracts, Testing, and Governance

**arXiv:** [2603.18096v1](https://arxiv.org/abs/2603.18096v1) · 2026-03-18 · cs.MA
**Authors:** Ciprian Paduraru, Petru-Liviu Bouruc, Alin Stefanescu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
In Agentic AI, Large Language Models (LLMs) are increasingly used in the orchestration layer to coordinate multiple agents and to interact with external services, retrieval components, and shared memory. In this setting, failures are not limited to incorrect final outputs. They also arise from long-horizon interaction, stochastic decisions, and external side effects (such as API calls, database writes, and message sends). Common failures include non-termination, role drift, propagation of unsupported claims, and attacks via untrusted context or external channels. This paper presents an assurance framework for such Agentic AI systems. Executions are instrumented as Message-Action Traces (MAT) with explicit step and trace contracts. Contracts provide machine-checkable verdicts, localize the first violating step, and support deterministic replay. The framework includes stress testing, formulated as a budgeted counterexample search over bounded perturbations. It also supports structured fault injection at service, retrieval, and memory boundaries to assess containment under realistic operational faults and degraded conditions. Finally, governance is treated as a runtime component, enforcing per-agent capability limits and action mediation (allow, rewrite, block) at the language-to-action boundary. To support comparative evaluations across stochastic seeds, models, and orchestration configurations, the paper defines trace-based metrics for task success, termination reliability, contract compliance, factuality indicators, containment rate, and governance outcome distributions. More broadly, the framework is intended as a common abstraction to support testing and evaluation of multi-agent LLM systems, and to facilitate reproducible comparison across orchestration designs and configurations.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.18096v1)
