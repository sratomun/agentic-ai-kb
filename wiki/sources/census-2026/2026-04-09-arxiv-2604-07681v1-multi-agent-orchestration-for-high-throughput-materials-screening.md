---
type: source
source_type: arxiv
title: "Multi-Agent Orchestration for High-Throughput Materials Screening on a Leadership-Class System"
authors: Thang Duc Pham, Harikrishna Tummalapalli, Fakhrul Hasan Bhuiyan, Álvaro Vázquez Mayagoitia et al.
url: https://arxiv.org/abs/2604.07681v1
date: 2026-04-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 30
primary: cs.AI
tags: [science-agents, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# Multi-Agent Orchestration for High-Throughput Materials Screening on a Leadership-Class System

**arXiv:** [2604.07681v1](https://arxiv.org/abs/2604.07681v1) · 2026-04-09 · cs.AI
**Authors:** Thang Duc Pham, Harikrishna Tummalapalli, Fakhrul Hasan Bhuiyan, Álvaro Vázquez Mayagoitia et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
The integration of Artificial Intelligence (AI) with High-Performance Computing (HPC) is transforming scientific workflows from human-directed pipelines into adaptive systems capable of autonomous decision-making. Large language models (LLMs) play a critical role in autonomous workflows; however, deploying LLM-based agents at scale remains a significant challenge. Single-agent architectures and sequential tool calls often become serialization bottlenecks when executing large-scale simulation campaigns, failing to utilize the massive parallelism of exascale resources. To address this, we present a scalable, hierarchical multi-agent framework for orchestrating high-throughput screening campaigns. Our planner-executor architecture employs a central planning agent to dynamically partition workloads and assign subtasks to a swarm of parallel executor agents. All executor agents interface with a shared Model Context Protocol (MCP) server that orchestrates tasks via the Parsl workflow engine. To demonstrate this framework, we employed the open-weight gpt-oss-120b model to orchestrate a high-throughput screening of the Computation-Ready Experimental (CoRE) Metal-Organic Framework (MOF) database for atmospheric water harvesting. The results demonstrate that the proposed agentic framework enables efficient and scalable execution on the Aurora supercomputer, with low orchestration overhead and high task completion rates. This work establishes a flexible paradigm for LLM-driven scientific automation on HPC systems, with broad applicability to materials discovery and beyond.

## Graph
- **Concepts:** [[science-agents|Science agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.07681v1)
