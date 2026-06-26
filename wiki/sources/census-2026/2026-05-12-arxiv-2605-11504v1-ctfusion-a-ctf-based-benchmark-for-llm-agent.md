---
type: source
source_type: arxiv
title: "CTFusion: A CTF-based Benchmark for LLM Agent Evaluation"
authors: Dongjun Lee, Ga-eun Bae, Insu Yun
url: https://arxiv.org/abs/2605.11504v1
date: 2026-05-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.LG
tags: [agent-reliability, agent-protocols, agent-evaluation, arxiv, auto-ingested]
---

# CTFusion: A CTF-based Benchmark for LLM Agent Evaluation

**arXiv:** [2605.11504v1](https://arxiv.org/abs/2605.11504v1) · 2026-05-12 · cs.LG
**Authors:** Dongjun Lee, Ga-eun Bae, Insu Yun

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Large Language Models (LLMs) have enabled agentic systems for complex, multi-step tasks; cybersecurity is emerging as a prominent application. To evaluate such agents, researchers widely adopt Capture The Flag (CTF) benchmarks. However, current CTF benchmarks reuse existing challenges, which exposes them to data contamination and potential cheating. Notably, we confirmed these issues in practice by integrating web search tools into an existing agent. To address these limitations, we present CTFusion, a streaming evaluation framework built on Live CTFs. To achieve this, CTFusion preserves per-agent independence under a single team account and reduces competition impact by forwarding only the first correct flag per challenge. Moreover, we implement CTFusion as a Model Context Protocol (MCP) server on the widely used CTFd platform, which offers broad applicability to diverse CTF events and agent types. Through experiments with three LLMs, two agents, and five Live CTFs, we demonstrate that existing CTF benchmarks can be unreliable in assessing LLM-based agents, while CTFusion can serve as a robust solution for evaluating cybersecurity agents. We release CTFusion as open source to foster future research in this area.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.11504v1)
