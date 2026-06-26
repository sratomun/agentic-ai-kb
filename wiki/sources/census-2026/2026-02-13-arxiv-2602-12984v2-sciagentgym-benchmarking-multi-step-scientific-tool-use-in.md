---
type: source
source_type: arxiv
title: "SciAgentGym: Benchmarking Multi-Step Scientific Tool-use in LLM Agents"
authors: Yujiong Shen, Yajie Yang, Zhiheng Xi, Binze Hu et al.
url: https://arxiv.org/abs/2602.12984v2
date: 2026-02-13
ingested: 2026-06-21
depth: abstract
auto: true
score: 20
primary: cs.CL
tags: [agent-memory, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# SciAgentGym: Benchmarking Multi-Step Scientific Tool-use in LLM Agents

**arXiv:** [2602.12984v2](https://arxiv.org/abs/2602.12984v2) · 2026-02-13 · cs.CL
**Authors:** Yujiong Shen, Yajie Yang, Zhiheng Xi, Binze Hu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Scientific reasoning inherently demands integrating sophisticated toolkits to navigate domain-specific knowledge. Yet, current benchmarks largely overlook agents' ability to orchestrate tools for such rigorous workflows. To bridge this gap, we introduce SciAgentGym, a scalable interactive environment featuring 1,780 domain-specific tools across four natural science disciplines, supported by a robust execution infrastructure. Complementing this, we present SciAgentBench, a tiered evaluation suite designed to stress-test agentic capabilities from elementary actions to long-horizon workflows. Our evaluation identifies a critical bottleneck: state-of-the-art models still struggle with complex scientific tool-use, and their performance degrades substantially as interaction horizons extend. To address this, we propose SciForge, a data synthesis method that models the tool action space as a dependency graph to generate logic-aware training trajectories. By fine-tuning on these trajectories, our SciAgent-8B outperforms the significantly larger Qwen3-VL-235B-Instruct while exhibiting positive cross-domain transfer of scientific tool-use capabilities. These results underscore the promising potential of next-generation autonomous scientific agents.

## Graph
- **Concepts:** [[agent-memory|Agent memory]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[qwen]] · [[agentbench]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2602.12984v2)
