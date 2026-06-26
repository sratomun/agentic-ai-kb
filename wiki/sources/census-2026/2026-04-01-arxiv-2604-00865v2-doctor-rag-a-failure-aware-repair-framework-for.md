---
type: source
source_type: arxiv
title: "Doctor-RAG: A Failure-Aware Repair Framework for Agentic Retrieval-Augmented Generation"
authors: Shuguang Jiao, Chengkai Huang, Shuhan Qi, Xuan Wang et al.
url: https://arxiv.org/abs/2604.00865v2
date: 2026-04-01
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.IR
tags: [clinical-agents, agent-reliability, agentic-rag, agent-evaluation, arxiv, auto-ingested]
---

# Doctor-RAG: A Failure-Aware Repair Framework for Agentic Retrieval-Augmented Generation

**arXiv:** [2604.00865v2](https://arxiv.org/abs/2604.00865v2) · 2026-04-01 · cs.IR
**Authors:** Shuguang Jiao, Chengkai Huang, Shuhan Qi, Xuan Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic Retrieval-Augmented Generation interleaves retrieval and reasoning for multi-hop QA and complex knowledge tasks. As reasoning trajectories lengthen, failures become more frequent, while existing methods often either stop at diagnosis or rely on coarse replanning and rerun-style recovery, incurring high computational cost. We propose DoctorRAG (DR-RAG), a diagnose-and-repair framework that corrects failures via explicit error localization and prefix reuse. DR-RAG operates in two stages: (i) trajectory-level failure diagnosis, where a distilled diagnosis model jointly assesses evidence sufficiency, classifies the failure type, and localizes the earliest failure point; and (ii) tool-conditioned local repair that intervenes only at the diagnosed point while reusing conditionally valid prefixes and retrieved evidence. By separating error attribution from correction, DR-RAG avoids blind reruns in a post-hoc repair setting and enables targeted, efficient correction of known failed trajectories. Experiments on three multi-hop QA benchmarks across multiple agentic RAG baselines and backbone models show substantial improvements in answer accuracy.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rag|Agentic RAG]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.00865v2)
