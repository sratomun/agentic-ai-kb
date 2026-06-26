---
type: entity
entity_type: benchmark
tags: [agents, benchmark, rca, reliability, evaluation]
created: 2026-06-22
updated: 2026-06-22
---

# Cloud-OpsBench

*A reproducible benchmark for agentic root-cause analysis on Kubernetes — 452 fault cases with process-centric metrics.*

## What it is
Cloud-OpsBench is a white-box benchmark for agentic RCA on Kubernetes (Wang et al., 2026): 452 fault cases across 40 root-cause types, all reproducible in seconds via a State Snapshot Paradigm that freezes the operational context into a deterministic digital twin. It introduces process-centric metrics beyond outcome accuracy.

## Why it matters
AI-driven ops automation is a high-value enterprise target. Cloud-OpsBench is the first rigorous benchmark that can tell 'right for the right reasons' from lucky answers — essential before trusting agents with production incident response.

## Relationships
- evaluates [[data-analysis-agents]]
- evaluates [[agent-reliability]]
- part of [[agent-evaluation]]

## Cited by
- [[2026-02-28-arxiv-2603-00468v1-cloud-opsbench-agentic-rca]]
