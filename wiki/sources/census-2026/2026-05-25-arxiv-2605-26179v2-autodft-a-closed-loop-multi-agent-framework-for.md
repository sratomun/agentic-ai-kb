---
type: source
source_type: arxiv
title: "AutoDFT: A Closed-Loop Multi-Agent Framework for Autonomous DFT Calculations"
authors: Penghui Yang, Zhonghan Zhang, Yue Li, Xinrun Wang et al.
url: https://arxiv.org/abs/2605.26179v2
date: 2026-05-25
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cond-mat.mtrl-sci
tags: [clinical-agents, science-agents, agent-reliability, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# AutoDFT: A Closed-Loop Multi-Agent Framework for Autonomous DFT Calculations

**arXiv:** [2605.26179v2](https://arxiv.org/abs/2605.26179v2) · 2026-05-25 · cond-mat.mtrl-sci
**Authors:** Penghui Yang, Zhonghan Zhang, Yue Li, Xinrun Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Density functional theory (DFT) serves as the basis for computational discovery in materials science and chemistry, yet each calculation demands extensive human effort: adjusting algorithms when convergence stalls, revising plans when unexpected physics emerges, and inserting steps as intermediate results reshape the problem. Existing LLM-based agents automate only the initial planning stage, producing a full execution plan upfront and leaving all subsequent adaptation to hand-crafted rules. As a result, these workflows remain fragile, do not generalize well beyond pre-planned scenarios, and often require expert intervention when failures or unexpected intermediate results require changes to the calculation path. Here, we introduce AutoDFT, a closed-loop multi-agent framework that embeds LLM reasoning into every stage of the DFT lifecycle, where a strategic planner produces a skeletal plan of step objectives; a step planner generates numerical parameters just in time from preceding results; and a monitor-recover-reflect cycle diagnoses failures, repairs them, and revises the plan when the evidence justifies it. We demonstrate both breadth and depth: breadth on VASPBench, a purpose-built benchmark spanning 34 tasks and 9 DFT calculation types, where AutoDFT achieves 94.1% task-level success with GPT-5.2; and depth on established materials databases, where AutoDFT produces quantitatively reliable property predictions across electronic, magnetic, and energetic properties. By closing the loop between planning and execution, AutoDFT enables experimentalists without deep computational expertise to obtain reliable first-principles results.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[agent-reliability|Agent reliability]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2605.26179v2)
