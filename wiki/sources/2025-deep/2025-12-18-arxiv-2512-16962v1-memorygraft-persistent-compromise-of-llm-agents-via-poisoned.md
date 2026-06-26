---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MemoryGraft: Persistent Compromise of LLM Agents via Poisoned Experience Retrieval"
authors: Saksham Sahai Srivastava, Haoyu He
url: https://arxiv.org/abs/2512.16962v1
date: 2025-12-18
citationCount: 36
influentialCitationCount: 5
velocity: 5.89
ingested: 2026-06-22
tags: [agent-reliability, self-evolving-agents, agent-security, agentic-rag, agent-memory, arxiv, 2025, cited]
---

# MemoryGraft: Persistent Compromise of LLM Agents via Poisoned Experience Retrieval

**arXiv [2512.16962v1](https://arxiv.org/abs/2512.16962v1)** · 2025-12-18 · **36 citations** (5 influential · 5.89/mo) · Saksham Sahai Srivastava, Haoyu He

## Abstract
Large Language Model (LLM) agents increasingly rely on long-term memory and Retrieval-Augmented Generation (RAG) to persist experiences and refine future performance. While this experience learning capability enhances agentic autonomy, it introduces a critical, unexplored attack surface, i.e., the trust boundary between an agent's reasoning core and its own past. In this paper, we introduce MemoryGraft. It is a novel indirect injection attack that compromises agent behavior not through immediate jailbreaks, but by implanting malicious successful experiences into the agent's long-term memory. Unlike traditional prompt injections that are transient, or standard RAG poisoning that targets factual knowledge, MemoryGraft exploits the agent's semantic imitation heuristic which is the tendency to replicate patterns from retrieved successful tasks. We demonstrate that an attacker who can supply benign ingestion-level artifacts that the agent reads during execution can induce it to construct a poisoned RAG store where a small set of malicious procedure templates is persisted alongside benign experiences. When the agent later encounters semantically similar tasks, union retrieval over lexical and embedding similarity reliably surfaces these grafted memories, and the agent adopts the embedded unsafe patterns, leading to persistent behavioral drift across sessions. We validate MemoryGraft on MetaGPT's DataInterpreter agent with GPT-4o and find that a small number of poisoned records can account for a large fraction of retrieved experiences on benign workloads, turning experience-based self-improvement into a vector for stealthy and durable compromise. To facilitate reproducibility and future research, our code and evaluation data are available at https://github.com/Jacobhhy/Agent-Memory-Poisoning.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Related Work Memory systems for LLM agents Prompt injection and RAG poisoning Memory injection and backdoor attacks 3 Threat Model 3.1 Agent Setting 3.2 Attacker’s Objectives 3.3 Realistic Constraints and Assumptions 4 Methodology 4.1 Attack Setup 4.2 Poisoning Phase 4.3 Evaluation Phase 4.4 Mechanism of Persistence and behavioral Drift 5 Experiment 5.1 Agent Configuration and Environment 5.2 Dataset Construction and Evaluation Protocol 5.3 Quantitative Results: Aggregate Retrieval 5.4 Mechanism Analysis: Impact of Union Retrieval (BM25+Embeddings) 5.5 Qualitative Analysis: Retrieval Dynamics 1. High retrieval penetration despite a small poisoned set 2. Robustness across heterogeneous user tasks 6 Potential Defense 7 Conclusion 8 Limitations and Future Work A Seed Set for RAG Vector-Drift Experiments B Evaluation Query Set C Additional Experiments Considered C.1 Schema-Spoofing Attack (ReAct Trace Injection) C.2 JudgeJacking Attack (Rubric-Mimicry) MemoryGraft: Persistent Compromise of…

**Method / approach.** Methodology 4.1 Attack Setup 4.2 Poisoning Phase 4.3 Evaluation Phase 4.4 Mechanism of Persistence and behavioral Drift 5 Experiment 5.1 Agent Configuration and Environment 5.2 Dataset Construction and Evaluation Protocol 5.3 Quantitative Results: Aggregate Retrieval 5.4 Mechanism Analysis: Impact of Union Retrieval (BM25+Embeddings) 5.5 Qualitative Analysis: Retrieval Dynamics 1. High retrieval penetration despite a small poisoned set 2. Robustness across heterogeneous user tasks 6 Potential Defense 7 Conclusion 8 Limitations and Future Work A Seed Set for RAG Vector-Drift Experiments B Evaluation Query Set C Additional Experiments Considered C.1 Schema-Spoofing Attack (ReAct Trace Injection) C.2 JudgeJacking Attack (Rubric-Mimicry) MemoryGraft: Persistent Compromise of LLM Agents via Poisoned Experience Retrieval Saksham Sahai Srivastava School of Computing University of Georgia Athens, GA 30602 saksham.srivastava@uga…

**Results.** Experiment 5.1 Agent Configuration and Environment 5.2 Dataset Construction and Evaluation Protocol 5.3 Quantitative Results: Aggregate Retrieval 5.4 Mechanism Analysis: Impact of Union Retrieval (BM25+Embeddings) 5.5 Qualitative Analysis: Retrieval Dynamics 1. High retrieval penetration despite a small poisoned set 2. Robustness across heterogeneous user tasks 6 Potential Defense 7 Conclusion 8 Limitations and Future Work A Seed Set for RAG Vector-Drift Experiments B Evaluation Query Set C Additional Experiments Considered C.1 Schema-Spoofing Attack (ReAct Trace Injection) C.2 JudgeJacking Attack (Rubric-Mimicry) MemoryGraft: Persistent Compromise of LLM Agents via Poisoned Experience Retrieval Saksham Sahai Srivastava School of Computing University of Georgia Athens, GA 30602 saksham.srivastava@uga.edu Haoyu He School of Computing University of Georgia Athens, GA 30602 haoyu.h…

**Conclusion.** Conclusion 8 Limitations and Future Work A Seed Set for RAG Vector-Drift Experiments B Evaluation Query Set C Additional Experiments Considered C.1 Schema-Spoofing Attack (ReAct Trace Injection) C.2 JudgeJacking Attack (Rubric-Mimicry) MemoryGraft: Persistent Compromise of LLM Agents via Poisoned Experience Retrieval Saksham Sahai Srivastava School of Computing University of Georgia Athens, GA 30602 saksham.srivastava@uga.edu Haoyu He School of Computing University of Georgia Athens, GA 30602 haoyu.he@uga.edu Abstract Large Language Model (LLM) agents increasingly rely on long-term memory and Retrieval-Augmented Generation (RAG) to persist experiences and refine future performance. While this experienc…

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[self-evolving-agents|Self-evolving agents]] · [[agent-security|Agent security]] · [[agentic-rag|Agentic RAG]] · [[agent-memory|Agent memory]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2512.16962v1.md` · `raw/arxiv/2512.16962v1.fulltext.md`
