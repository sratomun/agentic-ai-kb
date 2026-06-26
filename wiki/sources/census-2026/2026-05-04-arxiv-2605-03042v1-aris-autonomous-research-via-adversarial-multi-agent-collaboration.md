---
type: source
source_type: arxiv
title: "ARIS: Autonomous Research via Adversarial Multi-Agent Collaboration"
authors: Ruofeng Yang, Yongcan Li, Shuai Li
url: https://arxiv.org/abs/2605.03042v1
date: 2026-05-04
ingested: 2026-06-21
depth: abstract
auto: true
score: 14
primary: cs.SE
tags: [recommendation-agents, self-evolving-agents, agent-security, agent-protocols, agent-skills, arxiv, auto-ingested]
---

# ARIS: Autonomous Research via Adversarial Multi-Agent Collaboration

**arXiv:** [2605.03042v1](https://arxiv.org/abs/2605.03042v1) · 2026-05-04 · cs.SE
**Authors:** Ruofeng Yang, Yongcan Li, Shuai Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
This report describes ARIS (Auto-Research-in-sleep), an open-source research harness for autonomous research, including its architecture, assurance mechanisms, and early deployment experience. The performance of agent systems built on LLMs depends on both the model weights and the harness around them, which governs what information to store, retrieve, and present to the model. For long-horizon research workflows, the central failure mode is not a visible breakdown but a plausible unsupported success: a long-running agent can produce claims whose evidential support is incomplete, misreported, or silently inherited from the executor's framing. Therefore, we present ARIS as a research harness that coordinates machine-learning research workflows through cross-model adversarial collaboration as a default configuration: an executor model drives forward progress while a reviewer from a different model family is recommended to critique intermediate artifacts and request revisions. ARIS has three architectural layers. The execution layer provides more than 65 reusable Markdown-defined skills, model integrations via MCP, a persistent research wiki for iterative reuse of prior findings, and deterministic figure generation. The orchestration layer coordinates five end-to-end workflows with adjustable effort settings and configurable routing to reviewer models. The assurance layer includes a three-stage process for checking whether experimental claims are supported by evidence: integrity verification, result-to-claim mapping, and claim auditing that cross-checks manuscript statements against the claim ledger and raw evidence, as well as a five-pass scientific-editing pipeline, mathematical-proof checks, and visual inspection of the rendered PDF. A prototype self-improvement loop records research traces and proposes harness improvements that are adopted only after reviewer approval.

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-security|Agent security]] · [[agent-protocols|Agent protocols]] · [[agent-skills|Agent skills]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.03042v1)
