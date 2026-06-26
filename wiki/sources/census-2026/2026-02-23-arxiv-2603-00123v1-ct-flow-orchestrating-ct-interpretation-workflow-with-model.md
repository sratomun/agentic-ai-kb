---
type: source
source_type: arxiv
title: "CT-Flow: Orchestrating CT Interpretation Workflow with Model Context Protocol Servers"
authors: Yannian Gu, Xizhuo Zhang, Linjie Mu, Yongrui Yu et al.
url: https://arxiv.org/abs/2603.00123v1
date: 2026-02-23
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.CV
tags: [clinical-agents, agent-protocols, tool-use, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# CT-Flow: Orchestrating CT Interpretation Workflow with Model Context Protocol Servers

**arXiv:** [2603.00123v1](https://arxiv.org/abs/2603.00123v1) · 2026-02-23 · cs.CV
**Authors:** Yannian Gu, Xizhuo Zhang, Linjie Mu, Yongrui Yu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in Large Vision-Language Models (LVLMs) have shown strong potential for multi-modal radiological reasoning, particularly in tasks like diagnostic visual question answering (VQA) and radiology report generation. However, most existing approaches for 3D CT analysis largely rely on static, single-pass inference. In practice, clinical interpretation is a dynamic, tool-mediated workflow where radiologists iteratively review slices and use measurement, radiomics, and segmentation tools to refine findings. To bridge this gap, we propose CT-Flow, an agentic framework designed for interoperable volumetric interpretation. By leveraging the Model Context Protocol (MCP), CT-Flow shifts from closed-box inference to an open, tool-aware paradigm. We curate CT-FlowBench, the first large-scale instruction-tuning benchmark tailored for 3D CT tool-use and multi-step reasoning. Built upon this, CT-Flow functions as a clinical orchestrator capable of decomposing complex natural language queries into automated tool-use sequences. Experimental evaluations on CT-FlowBench and standard 3D VQA datasets demonstrate that CT-Flow achieves state-of-the-art performance, surpassing baseline models by 41% in diagnostic accuracy and achieving a 95% success rate in autonomous tool invocation. This work provides a scalable foundation for integrating autonomous, agentic intelligence into real-world clinical radiology.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[mcp]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00123v1)
