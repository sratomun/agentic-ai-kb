---
type: source
source_type: arxiv
title: "Agentic Mixed-Source Multi-Modal Misinformation Detection with Adaptive Test-Time Scaling"
authors: Wei Jiang, Tong Chen, Wei Yuan, Quoc Viet Hung Nguyen et al.
url: https://arxiv.org/abs/2603.02519v1
date: 2026-03-03
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.MM
tags: [multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Agentic Mixed-Source Multi-Modal Misinformation Detection with Adaptive Test-Time Scaling

**arXiv:** [2603.02519v1](https://arxiv.org/abs/2603.02519v1) · 2026-03-03 · cs.MM
**Authors:** Wei Jiang, Tong Chen, Wei Yuan, Quoc Viet Hung Nguyen et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Vision-language models (VLMs) have been proven effective for detecting multi-modal misinformation on social platforms, especially in zero-shot settings with unavailable or delayed annotations. However, a single VLM's capacity falls short in the more complex mixed-source multi-modal misinformation detection (M3D) task. Taking captioned images as an example, in M3D, false information can originate from untruthful texts, forged images, or mismatches between the two modalities. Although recent agentic systems can handle zero-shot M3D by connecting modality-specific VLM agents, their effectiveness is still bottlenecked by their architecture. In existing agentic M3D solutions, for any input sample, each agent performs only one forward reasoning pass, making decisions prone to model randomness and reasoning errors in challenging cases. Moreover, the lack of exploration over alternative reasoning paths prevents modern VLMs from fully utilizing their reasoning capacity. In this work, we present AgentM3D, a multi-agent framework for zero-shot M3D. To amplify the reasoning capability of VLMs, we introduce an adaptive test-time scaling paradigm in which each modality-specific VLM agent applies a Best-of-N mechanism, coupled with a critic agent for task-aligned scoring. The agents are organized in a cascading, modality-specific decision chain to reduce unnecessary computation and limit error propagation. To ensure scalability, a planning agent dynamically determines the maximum number of reasoning paths based on sample difficulty, and an adaptive stopping mechanism prevents excessive reasoning within each agent. Extensive experiments on two M3D benchmarks demonstrate that AgentM3D achieves state-of-the-art zero-shot detection performance compared with various VLM-based and agentic baselines.

## Graph
- **Concepts:** [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.02519v1)
