---
type: source
source_type: arxiv
title: "Large Language Models for Agentic NetOps and AIOps: Architectures, Evaluation, and Safety"
authors: Muhammad Bilal, Jon Crowcroft, Ruizhi Wang, Xiaolong Xu et al.
url: https://arxiv.org/abs/2605.12729v2
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.NI
tags: [recommendation-agents, clinical-agents, agent-reliability, agent-security, tool-use, arxiv, auto-ingested]
---

# Large Language Models for Agentic NetOps and AIOps: Architectures, Evaluation, and Safety

**arXiv:** [2605.12729v2](https://arxiv.org/abs/2605.12729v2) · 2026-05-12 · cs.NI
**Authors:** Muhammad Bilal, Jon Crowcroft, Ruizhi Wang, Xiaolong Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models are increasingly being used to support network operations (NetOps) and artificial intelligence for IT operations (AIOps), including incident investigation, root-cause analysis, configuration synthesis, and limited self-healing. In both NetOps and AIOps, this shift is changing how tasks are managed. Agent-based operations work as workflows, from gathering evidence to taking action, following permissions, policies, and checks, and providing rollback options when necessary. This is crucial because operational decisions can have instant impacts. To make the argument concrete, we organise the relevant literature around the hierarchy of autonomy, tool scope, evidence traces, and assurance contracts. These contracts define what an agent may observe, propose, and execute. They also define the checks that must pass before any action is allowed. A consistent pattern appears across work on telemetry query recommendation, diagnosis, root-cause analysis, configuration synthesis, change planning, and limited self-healing. Operational reliability does not come chiefly from the model itself. It depends on the machinery around the model. We also argue that evaluation should go beyond static question answering. Agentic NetOps and AIOps systems require workflow-centred evaluation, including trace quality, bounded tool use, safe proposal generation, replay in sandboxed environments, and canary trials with rollback-aware scoring. Without these measures, a system may appear robust yet remain too fragile. Finally, we examine security, privacy, and governance risks that become acute when agents sit close to operational control surfaces. Taken together, the survey concludes that progress in intelligent NetOps and AIOps will depend on treating autonomy as a constrained operational control problem, whose outputs must be reliable, auditable, and securely deployable.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[tool-use|Tool use]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.12729v2)
