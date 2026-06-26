---
type: source
source_type: arxiv
title: "RAGEN-2: Reasoning Collapse in Agentic RL"
authors: Zihan Wang, Chi Gui, Xing Jin, Qineng Wang et al.
url: https://arxiv.org/abs/2604.06268v1
date: 2026-04-07
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.LG
tags: [clinical-agents, computer-use-agents, embodied-agents, agent-reliability, agentic-rl, arxiv, auto-ingested]
---

# RAGEN-2: Reasoning Collapse in Agentic RL

**arXiv:** [2604.06268v1](https://arxiv.org/abs/2604.06268v1) · 2026-04-07 · cs.LG
**Authors:** Zihan Wang, Chi Gui, Xing Jin, Qineng Wang et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
RL training of multi-turn LLM agents is inherently unstable, and reasoning quality directly determines task performance. Entropy is widely used to track reasoning stability. However, entropy only measures diversity within the same input, and cannot tell whether reasoning actually responds to different inputs. In RAGEN-2, we find that even with stable entropy, models can rely on fixed templates that look diverse but are input-agnostic. We call this template collapse, a failure mode invisible to entropy and all existing metrics. To diagnose this failure, we decompose reasoning quality into within-input diversity (Entropy) and cross-input distinguishability (Mutual Information, MI), and introduce a family of mutual information proxies for online diagnosis. Across diverse tasks, mutual information correlates with final performance much more strongly than entropy, making it a more reliable proxy for reasoning quality. We further explain template collapse with a signal-to-noise ratio (SNR) mechanism. Low reward variance weakens task gradients, letting regularization terms dominate and erase cross-input reasoning differences. To address this, we propose SNR-Aware Filtering to select high-signal prompts per iteration using reward variance as a lightweight proxy. Across planning, math reasoning, web navigation, and code execution, the method consistently improves both input dependence and task performance.

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.06268v1)
