---
type: source
source_type: arxiv
title: "TopoEvo: A Topology-Aware Self-Evolving Multi-Agent Framework for Root Cause Analysis in Microservices"
authors: Junle Wang, Xingchuang Liao, Wenjun Wu
url: https://arxiv.org/abs/2605.15611v1
date: 2026-05-15
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [science-agents, agent-reliability, self-evolving-agents, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# TopoEvo: A Topology-Aware Self-Evolving Multi-Agent Framework for Root Cause Analysis in Microservices

**arXiv:** [2605.15611v1](https://arxiv.org/abs/2605.15611v1) · 2026-05-15 · cs.AI
**Authors:** Junle Wang, Xingchuang Liao, Wenjun Wu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Root cause analysis (RCA) in microservices is challenging due to (i) noisy and heterogeneous multimodal observability (metrics, logs, traces), (ii) cascading failure propagation that amplifies downstream symptoms, and (iii) non-stationary topology drift induced by autoscaling and rolling updates. Recent LLM-based RCA agents can generate tool-grounded explanations, yet they often remain topology-agnostic and suffer from \emph{symptom-amplification bias}, misattributing the root cause to salient downstream victims. We propose \textbf{TopoEvo}, a topology-aware self-evolving multi-agent framework that couples graph representation learning with structured, topology-constrained reasoning. TopoEvo first introduces \emph{Metric-orthogonal Multimodal Alignment} (MOMA), which decomposes metric embeddings into complementary subspaces and contrastively aligns logs and traces to reduce modality redundancy and sparsity, yielding stable node representations for graph encoding. It then applies \emph{Vector Quantization} (VQ) to discretize topology-enhanced states into auditable \emph{symptom tokens} with a symptom lexicon, enabling reliable retrieval and token-level evidence grounding. On top of these discrete topology cues, TopoEvo performs a multi-agent \emph{Hypothesis--Evidence--Test} (HET) workflow to explicitly verify propagation-consistent explanations and separate initiating anomalies from amplified downstream symptoms. Finally, a \emph{Self-Evolving Mechanism} refreshes hierarchical incident memory and performs conservative test-time adaptation with high-confidence pseudo-labels to maintain robustness under drift.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.15611v1)
