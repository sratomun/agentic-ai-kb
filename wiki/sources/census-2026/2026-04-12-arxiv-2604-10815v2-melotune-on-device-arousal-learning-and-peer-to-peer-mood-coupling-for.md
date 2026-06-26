---
type: source
source_type: arxiv
depth: abstract
auto: true
title: "MeloTune: On-Device Arousal Learning and Peer-to-Peer Mood Coupling for Proactive Music Curation"
authors: Hongwei Xu
url: https://arxiv.org/abs/2604.10815v2
date: 2026-04-12
score: 0
primary: cs.SD
tags: [arxiv, auto-ingested, small-language-models, agent-memory, clinical-agents, intent-routing]
---

# MeloTune: On-Device Arousal Learning and Peer-to-Peer Mood Coupling for Proactive Music Curation

**arXiv:** [2604.10815v2](https://arxiv.org/abs/2604.10815v2) · 2026-04-12 · cs.SD
**Authors:** Hongwei Xu

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
MeloTune is an iPhone-deployed music agent that instantiates the Mesh Memory Protocol (MMP) and Symbolic-Vector Attention Fusion (SVAF) as a production system for affect-aware music curation with peer-to-peer mood coupling. Each device runs two closed-form continuous-time (CfC) networks: a private listener-level CfC that predicts a short-horizon affective trajectory on Russell's circumplex and drives proactive curation, and a shared mesh-runtime CfC at MMP Layer 6 that integrates Cognitive Memory Blocks (CMBs) from co-listening peers. CfC hidden states never cross the wire; only structured CMBs do. A Personal Arousal Function (PAF) replaces the standard linear mapping from audio intensity to psychological arousal with a per-listener learned adjustment, trained from behavioral signals (skip, completion, favorite, volume) and from drift between user-declared mood and machine inference. The same track receives different arousal predictions for different listeners. The model (94,552 parameters) achieves trajectory MAE 0.414, pattern accuracy 96.6%, and intent accuracy 69.4% on held-out validation. PAF evidence from a live deployment session (46 observations across 11 genres) demonstrates that the learning loop operates end-to-end, with pop reaching full confidence after 22 observations. All inference runs on-device via CoreML. To our knowledge, this is the first production deployment of MMP/SVAF on consumer mobile hardware. The accompanying SDK (sym-swift v0.3.78, SYMCore v0.3.7) enforces strict protocol conformance. Music is the case study; the substrate is the contribution.

## Graph
- **Concepts:** [[small-language-models|Small Language Models]] · [[agent-memory]] · [[clinical-agents]] · [[intent-routing]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.10815v2)
