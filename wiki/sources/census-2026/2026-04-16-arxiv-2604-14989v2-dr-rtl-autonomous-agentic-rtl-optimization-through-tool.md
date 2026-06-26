---
type: source
source_type: arxiv
title: "Dr. RTL: Autonomous Agentic RTL Optimization through Tool-Grounded Self-Improvement"
authors: Wenji Fang, Yao Lu, Shang Liu, Jing Wang et al.
url: https://arxiv.org/abs/2604.14989v2
date: 2026-04-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 22
primary: cs.AI
tags: [self-evolving-agents, agent-skills, multi-agent-systems, arxiv, auto-ingested]
---

# Dr. RTL: Autonomous Agentic RTL Optimization through Tool-Grounded Self-Improvement

**arXiv:** [2604.14989v2](https://arxiv.org/abs/2604.14989v2) · 2026-04-16 · cs.AI
**Authors:** Wenji Fang, Yao Lu, Shang Liu, Jing Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Recent advances in large language models (LLMs) have sparked growing interest in automatic RTL optimization for better performance, power, and area (PPA). However, existing methods are still far from realistic RTL optimization. Their evaluation settings are often unrealistic: they are tested on manually degraded, small-scale RTL designs and rely on weak open-source tools. Their optimization methods are also limited, relying on coarse design-level feedback and simple pre-defined rewriting rules. To address these limitations, we present Dr. RTL, an agentic framework for RTL timing optimization in a realistic evaluation environment, with continual self-improvement through reusable optimization skills. We establish a realistic evaluation setting with more challenging RTL designs and an industrial EDA workflow. Within this setting, Dr. RTL performs closed-loop optimization through a multi-agent framework for critical-path analysis, parallel RTL rewriting, and tool-based evaluation. We further introduce group-relative skill learning, which compares parallel RTL rewrites and distills the optimization experience into an interpretable skill library. Currently, this library contains 47 pattern--strategy entries for cross-design reuse to improve PPA and accelerate convergence, and it can continue evolving over time. Evaluated on 20 real-world RTL designs, Dr. RTL achieves average WNS/TNS improvements of 21%/17% with a 6% area reduction over the industry-leading commercial synthesis tool.

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agent-skills|Agent skills]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.14989v2)
