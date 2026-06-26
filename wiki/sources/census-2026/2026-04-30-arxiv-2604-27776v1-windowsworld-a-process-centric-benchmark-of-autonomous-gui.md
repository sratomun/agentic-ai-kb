---
type: source
source_type: arxiv
title: "WindowsWorld: A Process-Centric Benchmark of Autonomous GUI Agents in Professional Cross-Application Environments"
authors: Jinchao Li, Yunxin Li, Chenrui Zhao, Zhenran Xu et al.
url: https://arxiv.org/abs/2604.27776v1
date: 2026-04-30
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.AI
tags: [computer-use-agents, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# WindowsWorld: A Process-Centric Benchmark of Autonomous GUI Agents in Professional Cross-Application Environments

**arXiv:** [2604.27776v1](https://arxiv.org/abs/2604.27776v1) · 2026-04-30 · cs.AI
**Authors:** Jinchao Li, Yunxin Li, Chenrui Zhao, Zhenran Xu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While GUI agents have shown impressive capabilities in common computer-use tasks such as OSWorld, current benchmarks mainly focus on isolated and single-application tasks. This overlooks a critical real-world requirement of coordinating across multiple applications to accomplish complex profession-specific workflows. To bridge this gap, we present a computer-use benchmark in cross-application workflows, named WindowsWorld, designed to systematically assess GUI Agents on complex multi-step tasks that mirror real-world professional activities. Our methodology uses a multi-agent framework steered by 16 occupations to generate four difficulty-level tasks with intermediate inspection, which are then refined by human review and executed in a simulated environment. The resulting benchmark contains 181 tasks with an average of 5.0 sub-goals across 17 common desktop applications, of which 78% are inherently multi-application. Experimental results of leading large models and agents show that: 1) All computer-use agents perform poorly on multi-application tasks (< 21% success rate), far below the performance of simple single-app tasks; 2) They largely fail at tasks requiring conditional judgment and reasoning across $\geq$ 3 applications, stalling at early sub-goals; 3) Low execution efficiency, where tasks often fail despite far exceeding human step limits. Code, benchmark data, and evaluation resources are available at github.com/HITsz-TMG/WindowsWorld.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[osworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.27776v1)
