---
type: source
source_type: arxiv
title: "Pushing the Limits of LLM Tool Calling via Experiential Knowledge Integration and Activation"
authors: Yupu Hao, Zhuoran Jin, Huanxuan Liao, Kang Liu et al.
url: https://arxiv.org/abs/2606.10875v1
date: 2026-06-09
ingested: 2026-06-21
depth: abstract
auto: true
score: 18
primary: cs.CL
tags: [agent-reliability, agentic-rl, tool-use, arxiv, auto-ingested]
---

# Pushing the Limits of LLM Tool Calling via Experiential Knowledge Integration and Activation

**arXiv:** [2606.10875v1](https://arxiv.org/abs/2606.10875v1) · 2026-06-09 · cs.CL
**Authors:** Yupu Hao, Zhuoran Jin, Huanxuan Liao, Kang Liu et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language models (LLMs) rely on tool use to act as autonomous agents, yet often fail in multi-step execution due to insufficient tool-related knowledge and ineffective knowledge activation. Therefore, we present a systematic study on how knowledge influences tool-use performance, covering the stages of knowledge acquisition, activation, and internalization. In the knowledge acquisition stage, we acquire and evaluate various forms of experiential knowledge, and our analysis shows that simple instance-level knowledge can already provide strong and reliable gains, while abstract intent-level knowledge offers limited benefits. At inference time, to activate knowledge, we find that prompting LLM to expand the depth of reasoning yields diminishing returns, whereas expanding the width of reasoning by parallel sampling with aggregation more effectively activates latent experiential knowledge. At training time, for knowledge internalization, post-training with knowledge-augmented data further improves performance, with reinforcement learning outperforming supervised fine-tuning. Based on these insights, we propose the Knowledge-Augmented Tool Execution (KATE), a knowledge-augmented tool execution framework that integrates experiential knowledge with reasoning-width-expanded inference and knowledge-aware training. Experiments on BFCL-V3 and AppWorld demonstrate consistent and substantial improvements over strong baselines across model scales. Our Code is available at https://github.com/hypasd-art/KATE.

## Graph
- **Concepts:** [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[tool-use|Tool use]]
- **Entities:** [[bfcl]] · [[appworld]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.10875v1)
