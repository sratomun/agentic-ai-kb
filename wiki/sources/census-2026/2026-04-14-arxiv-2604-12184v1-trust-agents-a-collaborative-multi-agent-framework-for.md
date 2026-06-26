---
type: source
source_type: arxiv
title: "TRUST Agents: A Collaborative Multi-Agent Framework for Fake News Detection, Explainable Verification, and Logic-Aware Claim Reasoning"
authors: Gautama Shastry Bulusu Venkata, Santhosh Kakarla, Maheedhar Omtri Mohan, Aishwarya Gaddam
url: https://arxiv.org/abs/2604.12184v1
date: 2026-04-14
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# TRUST Agents: A Collaborative Multi-Agent Framework for Fake News Detection, Explainable Verification, and Logic-Aware Claim Reasoning

**arXiv:** [2604.12184v1](https://arxiv.org/abs/2604.12184v1) · 2026-04-14 · cs.AI
**Authors:** Gautama Shastry Bulusu Venkata, Santhosh Kakarla, Maheedhar Omtri Mohan, Aishwarya Gaddam

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
TRUST Agents is a collaborative multi-agent framework for explainable fact verification and fake news detection. Rather than treating verification as a simple true-or-false classification task, the system identifies verifiable claims, retrieves relevant evidence, compares claims against that evidence, reasons under uncertainty, and generates explanations that humans can inspect. The baseline pipeline consists of four specialized agents. A claim extractor uses named entity recognition, dependency parsing, and LLM-based extraction to identify factual claims. A retrieval agent performs hybrid sparse and dense search using BM25 and FAISS. A verifier agent compares claims with retrieved evidence and produces verdicts with calibrated confidence. An explainer agent then generates a human-readable report with explicit evidence citations. To handle complex claims more effectively, we introduce a research-oriented extension with three additional components: a decomposer agent inspired by LoCal-style claim decomposition, a Delphi-inspired multi-agent jury with specialized verifier personas, and a logic aggregator that combines atomic verdicts using conjunction, disjunction, negation, and implication. We evaluate both pipelines on the LIAR benchmark against fine-tuned BERT, fine-tuned RoBERTa, and a zero-shot LLM baseline. Although supervised encoders remain stronger on raw metrics, TRUST Agents improves interpretability, evidence transparency, and reasoning over compound claims. Results also show that retrieval quality and uncertainty calibration remain the main bottlenecks in trustworthy automated fact verification.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.12184v1)
