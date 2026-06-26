---
type: source
source_type: arxiv
title: "GUITester: Enabling GUI Agents for Exploratory Defect Discovery"
authors: Yifei Gao, Jiang Wu, Xiaoyi Chen, Yifan Yang et al.
url: https://arxiv.org/abs/2601.04500v1
date: 2026-01-08
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [computer-use-agents, embodied-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# GUITester: Enabling GUI Agents for Exploratory Defect Discovery

**arXiv:** [2601.04500v1](https://arxiv.org/abs/2601.04500v1) · 2026-01-08 · cs.AI
**Authors:** Yifei Gao, Jiang Wu, Xiaoyi Chen, Yifan Yang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Exploratory GUI testing is essential for software quality but suffers from high manual costs. While Multi-modal Large Language Model (MLLM) agents excel in navigation, they fail to autonomously discover defects due to two core challenges: \textit{Goal-Oriented Masking}, where agents prioritize task completion over reporting anomalies, and \textit{Execution-Bias Attribution}, where system defects are misidentified as agent errors. To address these, we first introduce \textbf{GUITestBench}, the first interactive benchmark for this task, featuring 143 tasks across 26 defects. We then propose \textbf{GUITester}, a multi-agent framework that decouples navigation from verification via two modules: (i) a \textit{Planning-Execution Module (PEM)} that proactively probes for defects via embedded testing intents, and (ii) a \textit{Hierarchical Reflection Module (HRM)} that resolves attribution ambiguity through interaction history analysis. GUITester achieves an F1-score of 48.90\% (Pass@3) on GUITestBench, outperforming state-of-the-art baselines (33.35\%). Our work demonstrates the feasibility of autonomous exploratory testing and provides a robust foundation for future GUI quality assurance~\footnote{Our code is now available in~\href{https://github.com/ADaM-BJTU/GUITestBench}{https://github.com/ADaM-BJTU/GUITestBench}}.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.04500v1)
