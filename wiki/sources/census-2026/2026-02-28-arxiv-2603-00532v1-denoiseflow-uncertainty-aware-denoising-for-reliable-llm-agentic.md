---
type: source
source_type: arxiv
title: "DenoiseFlow: Uncertainty-Aware Denoising for Reliable LLM Agentic Workflows"
authors: Yandong Yan, Junwei Peng, Shijie Li, Chenxi Li et al.
url: https://arxiv.org/abs/2603.00532v1
date: 2026-02-28
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [coding-agents, agent-reliability, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# DenoiseFlow: Uncertainty-Aware Denoising for Reliable LLM Agentic Workflows

**arXiv:** [2603.00532v1](https://arxiv.org/abs/2603.00532v1) · 2026-02-28 · cs.AI
**Authors:** Yandong Yan, Junwei Peng, Shijie Li, Chenxi Li et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Autonomous agents are increasingly entrusted with complex, long-horizon tasks, ranging from mathematical reasoning to software generation. While agentic workflows facilitate these tasks by decomposing them into multi-step reasoning chains, reliability degrades significantly as the sequence lengthens. Specifically, minor interpretation errors in natural-language instructions tend to compound silently across steps. We term this failure mode accumulated semantic ambiguity. Existing approaches to mitigate this often lack runtime adaptivity, relying instead on static exploration budgets, reactive error recovery, or single-path execution that ignores uncertainty entirely. We formalize the multi-step reasoning process as a Noisy MDP and propose DenoiseFlow, a closed-loop framework that performs progressive denoising through three coordinated stages: (1)Sensing estimates per-step semantic uncertainty; (2)Regulating adaptively allocates computation by routing between fast single-path execution and parallel exploration based on estimated risk; and (3)Correcting performs targeted recovery via influence-based root-cause localization. Online self-calibration continuously aligns decision boundaries with verifier feedback, requiring no ground-truth labels. Experiments on six benchmarks spanning mathematical reasoning, code generation, and multi-hop QA show that DenoiseFlow achieves the highest accuracy on every benchmark (83.3% average, +1.3% over the strongest baseline) while reducing cost by 40--56% through adaptive branching. Detailed ablation studies further confirm framework-level's robustness and generality. Code is available at https://anonymous.4open.science/r/DenoiseFlow-21D3/.

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agent-reliability|Agent reliability]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00532v1)
