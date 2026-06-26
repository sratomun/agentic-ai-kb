---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "A-MemGuard: A Proactive Defense Framework for LLM-Based Agent Memory"
authors: Qianshan Wei, Tengchao Yang, Yaochen Wang, Xinfeng Li et al.
url: https://arxiv.org/abs/2510.02373v1
date: 2025-09-29
citationCount: 36
influentialCitationCount: 3
velocity: 4.12
ingested: 2026-06-22
tags: [embodied-agents, agent-reliability, agent-security, agent-memory, agent-evaluation, arxiv, 2025, cited]
---

# A-MemGuard: A Proactive Defense Framework for LLM-Based Agent Memory

**arXiv [2510.02373v1](https://arxiv.org/abs/2510.02373v1)** · 2025-09-29 · **36 citations** (3 influential · 4.12/mo) · Qianshan Wei, Tengchao Yang, Yaochen Wang, Xinfeng Li et al.

## Abstract
Large Language Model (LLM) agents use memory to learn from past interactions, enabling autonomous planning and decision-making in complex environments. However, this reliance on memory introduces a critical security risk: an adversary can inject seemingly harmless records into an agent's memory to manipulate its future behavior. This vulnerability is characterized by two core aspects: First, the malicious effect of injected records is only activated within a specific context, making them hard to detect when individual memory entries are audited in isolation. Second, once triggered, the manipulation can initiate a self-reinforcing error cycle: the corrupted outcome is stored as precedent, which not only amplifies the initial error but also progressively lowers the threshold for similar attacks in the future. To address these challenges, we introduce A-MemGuard (Agent-Memory Guard), the first proactive defense framework for LLM agent memory. The core idea of our work is the insight that memory itself must become both self-checking and self-correcting. Without modifying the agent's core architecture, A-MemGuard combines two mechanisms: (1) consensus-based validation, which detects anomalies by comparing reasoning paths derived from multiple related memories and (2) a dual-memory structure, where detected failures are distilled into ``lessons'' stored separately and consulted before future actions, breaking error cycles and enabling adaptation. Comprehensive evaluations on multiple benchmarks show that A-MemGuard effectively cuts attack success rates by over 95% while incurring a minimal utility cost. This work shifts LLM memory security from static filtering to a proactive, experience-driven model where defenses strengthen over time. Our code is available in https://github.com/TangciuYueng/AMemGuard

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work 3 Preliminary 3.1 Memory-Augmented Agent Architecture 3.2 Threat Model 3.3 Problem Formulation 4 Methodology: A-MemGuard Framework 4.1 Consensus Validation via Reasoning Path Analysis Parallel Reasoning Path Generation. Path Divergence Scoring and Validation. 4.2 Self-Taught Correction via Dual-Memory Structure Structured Lesson Distillation. Proactive Deliberation and Action Revision. 5 Experiments 5.1 Experimental Setup 5.2 Effectiveness at defending against direct injection methods 5.3 Effectiveness at defending against indirect injection methods 5.4 Utility cost of A-MemGuard on benign tasks 5.5 Scalability of our defense to collaborative multi-agent systems 5.6 Ablation Study 5.7 Hyperparameter Sensitivity Analysis 5.8 Why Consensus-Based Validation Works 6 Conclusion 7 Ethics Statement 8 Reproducibility Statement A Implementation Details for the Validation Module A.1 Instantiation 1: LLM-based Direct Decision-Making (Main Method) Operational Mechanics. A.2 Instantiation 2: V…

**Method / approach.** Methodology: A-MemGuard Framework 4.1 Consensus Validation via Reasoning Path Analysis Parallel Reasoning Path Generation. Path Divergence Scoring and Validation. 4.2 Self-Taught Correction via Dual-Memory Structure Structured Lesson Distillation. Proactive Deliberation and Action Revision. 5 Experiments 5.1 Experimental Setup 5.2 Effectiveness at defending against direct injection methods 5.3 Effectiveness at defending against indirect injection methods 5.4 Utility cost of A-MemGuard on benign tasks 5.5 Scalability of our defense to collaborative multi-agent systems 5.6 Ablation Study 5.7 Hyperparameter Sensitivity Analysis 5.8 Why Consensus-Based Validation Works 6 Conclusion 7 Ethics Statement 8 Reproducibility Statement A Implementation Details for the Validation Module A.1 Instantiation 1: LLM-based Direct Decision-Making (Main Method) Operational Mechanics. A.2 Instantiation 2: Validation via Embedding Distance Meth…

**Results.** Experiments 5.1 Experimental Setup 5.2 Effectiveness at defending against direct injection methods 5.3 Effectiveness at defending against indirect injection methods 5.4 Utility cost of A-MemGuard on benign tasks 5.5 Scalability of our defense to collaborative multi-agent systems 5.6 Ablation Study 5.7 Hyperparameter Sensitivity Analysis 5.8 Why Consensus-Based Validation Works 6 Conclusion 7 Ethics Statement 8 Reproducibility Statement A Implementation Details for the Validation Module A.1 Instantiation 1: LLM-based Direct Decision-Making (Main Method) Operational Mechanics. A.2 Instantiation 2: Validation via Embedding Distance Methodology. Analysis of Threshold Sensitivity. A.3 Instantiation 3: Validation via Density-Based Clustering (DBSCAN) Methodology. Analysis of Threshold Sensitivity. B Baseline Implementation Details B.1 LLM-based Memory Auditor B.2 Distil Classifi…

**Conclusion.** Conclusion 7 Ethics Statement 8 Reproducibility Statement A Implementation Details for the Validation Module A.1 Instantiation 1: LLM-based Direct Decision-Making (Main Method) Operational Mechanics. A.2 Instantiation 2: Validation via Embedding Distance Methodology. Analysis of Threshold Sensitivity. A.3 Instantiation 3: Validation via Density-Based Clustering (DBSCAN) Methodology. Analysis of Threshold Sensitivity. B Baseline Implementation Details B.1 LLM-based Memory Auditor B.2 Distil Classifier Dataset and Preprocessing. Training and Optimization. B.3 Perplexity Filter (PPL) Perplexity Score Calculation. Two-Stage Filtering Mechanism. C Knowledge Graph Construction and Anal…

## Graph
- **Concepts:** [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[a-mem]]
- **Raw:** `raw/arxiv/2510.02373v1.md` · `raw/arxiv/2510.02373v1.fulltext.md`
