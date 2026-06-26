---
type: source
source_type: arxiv
title: "CuraView: A Multi-Agent Framework for Medical Hallucination Detection with GraphRAG-Enhanced Knowledge Verification"
authors: Severin Ye, Xiao Kong, Xiaopeng He, Guangsu Yan et al.
url: https://arxiv.org/abs/2605.03476v1
date: 2026-05-05
ingested: 2026-06-21
depth: abstract
auto: true
score: 13
primary: cs.CL
tags: [clinical-agents, knowledge-graph, agent-reliability, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# CuraView: A Multi-Agent Framework for Medical Hallucination Detection with GraphRAG-Enhanced Knowledge Verification

**arXiv:** [2605.03476v1](https://arxiv.org/abs/2605.03476v1) · 2026-05-05 · cs.CL
**Authors:** Severin Ye, Xiao Kong, Xiaopeng He, Guangsu Yan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Discharge summaries require extracting critical information from lengthy electronic health records (EHRs), a process that is labor-intensive when performed manually. Large language models (LLMs) can improve generation efficiency; however, they are prone to producing faithfulness hallucinations, statements that contradict source records, posing direct risks to patient safety. To address this, we present CuraView, a multi-agent framework for sentence-level detection and evidence-grounded explanation of faithfulness hallucinations in discharge summaries. CuraView constructs a GraphRAG-based knowledge graph from patient-level EHRs and implements a closed-loop generation-detection pipeline with sentence-level evidence retrieval and classification spanning four evidence grades from strong support to direct contradiction (E1-E4), yielding structured and interpretable evidence chains. We evaluate CuraView on a subset of 250 patients from the Discharge-Me benchmark, with 50 patients held out for testing. Our fine-tuned Qwen3-14B detection model achieves an F1 of 0.831 on the safety-critical E4 metric (90.9% recall, 76.5% precision) and an F1 of 0.823 on E3+E4, representing a 50.0% relative improvement over the base model and outperforming RAGTruth-style and QAGS-style baselines. These results demonstrate that evidence-chain-based graph retrieval verification substantially improves the factual reliability of clinical documentation, while simultaneously producing reusable annotated datasets for downstream model training and distillation.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[graphrag]] · [[qwen]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.03476v1)
