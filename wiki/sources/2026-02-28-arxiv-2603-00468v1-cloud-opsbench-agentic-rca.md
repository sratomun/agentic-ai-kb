---
type: source
source_type: arxiv
title: "Cloud-OpsBench: A Reproducible Benchmark for Agentic Root Cause Analysis in Cloud Systems"
authors: Yilun Wang, Guangba Yu, Haiyu Huang, Zirui Wang, Yujie Huang, Pengfei Chen, Michael R. Lyu
url: https://arxiv.org/abs/2603.00468v1
date: 2026-02-28
ingested: 2026-06-22
depth: full-text
tags: [agent-evaluation, agent-reliability, data-analysis-agents, arxiv]
---

# Cloud-OpsBench: A Reproducible Benchmark for Agentic Root Cause Analysis in Cloud Systems

**Why it matters:** The clearest 2026 statement of *how* to evaluate a root-cause-analysis agent: stop scoring only the final answer (which rewards being "right for the wrong reasons") and score the **diagnostic trajectory** — did the agent gather evidence in a logical order. A deterministic digital twin makes runs 100% reproducible.

## What it is
A white-box, reproducible benchmark for agentic RCA on Kubernetes. A **State Snapshot Paradigm** freezes the full operational context (control-plane objects, metrics, logs) into an immutable digital twin served via mocked, zero-latency tools (e.g. `kubectl`) — so agents interact and probe, but state transitions are deterministic. **452 fault cases across 40 root-cause types**, full K8s stack. Evaluated 7 models in two tiers: LLM tier (GPT-5, GPT-4o, Claude-4-Sonnet, DeepSeek-V3.2, Qwen3-235B) and SLM tier (Qwen3-14B, Qwen3-8B).

## Metrics (this is the contribution)
- **Outcome:** A@1 / A@3 top-k accuracy (a diagnosis is correct only if stage + faulty component + failure reason all match); **TCR** (Task Completion Rate — outputs a valid structured diagnosis without crashing).
- **Process:** Trajectory Alignment in three strictnesses — Exact / Any-Order / In-Order Match vs expert reference paths; **Tool Relevance** & **Tool Coverage**; **Redundant Action Rate (RAR)**; Steps; **Invalid Action Count (IAC)**; **Zero-Tool Diagnosis Rate (ZTDR)**.

## Findings
- **Performance stratifies by symptom explicitness:** explicit faults (CrashLoopBackOff, OOMKilled) average A@1 > 0.65; implicit faults (resource contention, requiring cross-layer causal inference) average A@1 < 0.36.
- **Any-Order > In-Order alignment** for all models (Qwen3-235B 0.41 vs 0.38): agents find the right evidence but struggle to order it into a linear deductive chain.
- **The "redundancy paradox":** best performer DeepSeek-V3.2 has the highest RAR (0.11) and is coverage-centric (Steps 10.0, Coverage 0.88) — redundant checks act as cognitive self-correction; GPT-4o's near-zero RAR (0.02) correlates with *worse*, more fragile reasoning. GPT-5 is relevance-centric (efficient).
- **Failure modes named:** Claude-4-Sonnet shows "laziness" — ZTDR 0.32, hallucinating a root cause from the alert text without investigating (A@1 = 0.5, avg 4.25 steps). SLMs show syntactic fragility, schema hallucination, and repetition loops (can't use error feedback to recover).
- **ICL (procedural demonstrations) > RAG (declarative docs)** for SRE knowledge; a 14B model with procedural demos can rival proprietary giants. Full benchmark run takes seconds on a laptop.

## So what
For data-analyst / RCA agents the headline metric is not "did it name a cause" — it's root-cause accuracy **plus** trajectory alignment, tool coverage, and redundancy. Cloud-OpsBench's deterministic twin is also the model for making any analytics-agent eval reproducible.

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[agent-reliability|Agent reliability]] · [[data-analysis-agents|Data-analysis agents]]
- **Entities:** [[cloud-opsbench]]
- **Raw:** alphaXiv full-text (id 2603.00468v1)

## Relationships
- benchmarks [[data-analysis-agents]]
- evaluates [[agent-reliability]]
- part of [[agent-evaluation]]
