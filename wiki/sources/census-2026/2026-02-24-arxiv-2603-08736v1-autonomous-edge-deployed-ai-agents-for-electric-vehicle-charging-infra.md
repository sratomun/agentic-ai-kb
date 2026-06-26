---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "Autonomous Edge-Deployed AI Agents for Electric Vehicle Charging Infrastructure Management"
authors: Mohammed Cherifi
url: https://arxiv.org/abs/2603.08736v1
date: 2026-02-24
score: 11
primary: cs.DC
tags: [arxiv, auto-ingested, small-language-models, llm-as-judge, post-training, reasoning-models, agentic-rag]
---

# Autonomous Edge-Deployed AI Agents for Electric Vehicle Charging Infrastructure Management

**arXiv:** [2603.08736v1](https://arxiv.org/abs/2603.08736v1) · 2026-02-24 · cs.DC
**Authors:** Mohammed Cherifi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Public EV charging infrastructure suffers from significant failure rates -- with field studies reporting up to 27.5% of DC fast chargers non-functional -- and multi-day mean time to resolution, imposing billions in annual economic burden. Cloud-centric architectures cannot achieve the latency, reliability, and bandwidth characteristics required for autonomous operation. We present Auralink SDC (Software-Defined Charging), an architecture deploying domain-specialized AI agents at the network edge for autonomous charging infrastructure management. Key contributions include: (1) Confidence-Calibrated Autonomous Resolution (CCAR), enabling autonomous remediation with formal false-positive bounds; (2) Adaptive Retrieval-Augmented Reasoning (ARA), combining dense and sparse retrieval with dynamic context allocation; (3) Auralink Edge Runtime, achieving sub-50ms TTFT on commodity hardware under PREEMPT_RT constraints; and (4) Hierarchical Multi-Agent Orchestration (HMAO). Implementation uses AuralinkLM models fine-tuned via QLoRA on a domain corpus spanning OCPP 1.6/2.0.1, ISO 15118, and operational incident histories. Evaluation on 18,000 labeled incidents in a controlled environment establishes 78% autonomous incident resolution, 87.6% diagnostic accuracy, and 28-48ms TTFT latency (P50). This work presents architecture and implementation patterns for edge-deployed industrial AI systems with safety-critical constraints.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[llm-as-judge]] · [[post-training]] · [[reasoning-models]] · [[agentic-rag]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.08736v1)
