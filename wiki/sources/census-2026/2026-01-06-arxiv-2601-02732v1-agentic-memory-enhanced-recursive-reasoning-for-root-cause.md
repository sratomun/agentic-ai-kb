---
type: source
source_type: arxiv
title: "Agentic Memory Enhanced Recursive Reasoning for Root Cause Localization in Microservices"
authors: Lingzhe Zhang, Tong Jia, Yunpeng Zhai, Leyi Pan et al.
url: https://arxiv.org/abs/2601.02732v1
date: 2026-01-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.SE
tags: [agent-reliability, agent-memory, multi-agent-systems, arxiv, auto-ingested]
---

# Agentic Memory Enhanced Recursive Reasoning for Root Cause Localization in Microservices

**arXiv:** [2601.02732v1](https://arxiv.org/abs/2601.02732v1) · 2026-01-06 · cs.SE
**Authors:** Lingzhe Zhang, Tong Jia, Yunpeng Zhai, Leyi Pan et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As contemporary microservice systems become increasingly popular and complex-often comprising hundreds or even thousands of fine-grained, interdependent subsystems-they are experiencing more frequent failures. Ensuring system reliability thus demands accurate root cause localization. While many traditional graph-based and deep learning approaches have been explored for this task, they often rely heavily on pre-defined schemas that struggle to adapt to evolving operational contexts. Consequently, a number of LLM-based methods have recently been proposed. However, these methods still face two major limitations: shallow, symptom-centric reasoning that undermines accuracy, and a lack of cross-alert reuse that leads to redundant reasoning and high latency. In this paper, we conduct a comprehensive study of how Site Reliability Engineers (SREs) localize the root causes of failures, drawing insights from professionals across multiple organizations. Our investigation reveals that expert root cause analysis exhibits three key characteristics: recursiveness, multi-dimensional expansion, and cross-modal reasoning. Motivated by these findings, we introduce AMER-RCL, an agentic memory enhanced recursive reasoning framework for root cause localization in microservices. AMER-RCL employs the Recursive Reasoning RCL engine, a multi-agent framework that performs recursive reasoning on each alert to progressively refine candidate causes, while Agentic Memory incrementally accumulates and reuses reasoning from prior alerts within a time window to reduce redundant exploration and lower inference latency. Experimental results demonstrate that AMER-RCL consistently outperforms state-of-the-art methods in both localization accuracy and inference efficiency.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.02732v1)
