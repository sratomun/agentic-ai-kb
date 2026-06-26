---
type: source
source_type: arxiv
title: "AutoVerifier: An Agentic Automated Verification Framework Using Large Language Models"
authors: Yuntao Du, Minh Dinh, Kaiyuan Zhang, Ninghui Li
url: https://arxiv.org/abs/2604.02617v1
date: 2026-04-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 10
primary: cs.AI
tags: [science-agents, knowledge-graph, agent-reliability, arxiv, auto-ingested]
---

# AutoVerifier: An Agentic Automated Verification Framework Using Large Language Models

**arXiv:** [2604.02617v1](https://arxiv.org/abs/2604.02617v1) · 2026-04-03 · cs.AI
**Authors:** Yuntao Du, Minh Dinh, Kaiyuan Zhang, Ninghui Li

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Scientific and Technical Intelligence (S&TI) analysis requires verifying complex technical claims across rapidly growing literature, where existing approaches fail to bridge the verification gap between surface-level accuracy and deeper methodological validity. We present AutoVerifier, an LLM-based agentic framework that automates end-to-end verification of technical claims without requiring domain expertise. AutoVerifier decomposes every technical assertion into structured claim triples of the form (Subject, Predicate, Object), constructing knowledge graphs that enable structured reasoning across six progressively enriching layers: corpus construction and ingestion, entity and claim extraction, intra-document verification, cross-source verification, external signal corroboration, and final hypothesis matrix generation. We demonstrate AutoVerifier on a contested quantum computing claim, where the framework, operated by analysts with no quantum expertise, automatically identified overclaims and metric inconsistencies within the target paper, traced cross-source contradictions, uncovered undisclosed commercial conflicts of interest, and produced a final assessment. These results show that structured LLM verification can reliably evaluate the validity and maturity of emerging technologies, turning raw technical documents into traceable, evidence-backed intelligence assessments.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[knowledge-graph|Knowledge graphs]] · [[agent-reliability|Agent reliability]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.02617v1)
