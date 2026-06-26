---
type: source
source_type: arxiv
title: "TraceSIR: A Multi-Agent Framework for Structured Analysis and Reporting of Agentic Execution Traces"
authors: Shu-Xun Yang, Cunxiang Wang, Haoke Zhang, Wenbo Yu et al.
url: https://arxiv.org/abs/2603.00623v1
date: 2026-02-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [clinical-agents, agent-reliability, agent-protocols, tool-use, multi-agent-systems, arxiv, auto-ingested]
---

# TraceSIR: A Multi-Agent Framework for Structured Analysis and Reporting of Agentic Execution Traces

**arXiv:** [2603.00623v1](https://arxiv.org/abs/2603.00623v1) · 2026-02-28 · cs.AI
**Authors:** Shu-Xun Yang, Cunxiang Wang, Haoke Zhang, Wenbo Yu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Agentic systems augment large language models with external tools and iterative decision making, enabling complex tasks such as deep research, function calling, and coding. However, their long and intricate execution traces make failure diagnosis and root cause analysis extremely challenging. Manual inspection does not scale, while directly applying LLMs to raw traces is hindered by input length limits and unreliable reasoning. Focusing solely on final task outcomes further discards critical behavioral information required for accurate issue localization. To address these issues, we propose TraceSIR, a multi-agent framework for structured analysis and reporting of agentic execution traces. TraceSIR coordinates three specialized agents: (1) StructureAgent, which introduces a novel abstraction format, TraceFormat, to compress execution traces while preserving essential behavioral information; (2) InsightAgent, which performs fine-grained diagnosis including issue localization, root cause analysis, and optimization suggestions; (3) ReportAgent, which aggregates insights across task instances and generates comprehensive analysis reports. To evaluate TraceSIR, we construct TraceBench, covering three real-world agentic scenarios, and introduce ReportEval, an evaluation protocol for assessing the quality and usability of analysis reports aligned with industry needs. Experiments show that TraceSIR consistently produces coherent, informative, and actionable reports, significantly outperforming existing approaches across all evaluation dimensions. Our project and video are publicly available at https://github.com/SHU-XUN/TraceSIR.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[agent-reliability|Agent reliability]] · [[agent-protocols|Agent protocols]] · [[tool-use|Tool use]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00623v1)
