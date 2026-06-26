---
type: source
source_type: arxiv
title: "Benchmarking Open-Ended Multi-Agent Coordination in Language Agents"
authors: Kale-ab Abebe Tessera, Andras Szecsenyi, Cameron Barker, Alexander Rutherford et al.
url: https://arxiv.org/abs/2606.08340v1
date: 2026-06-06
ingested: 2026-06-21
depth: abstract
auto: true
score: 21
primary: cs.AI
tags: [agentic-rl, agent-memory, multi-agent-systems, agent-evaluation, arxiv, auto-ingested]
---

# Benchmarking Open-Ended Multi-Agent Coordination in Language Agents

**arXiv:** [2606.08340v1](https://arxiv.org/abs/2606.08340v1) · 2026-06-06 · cs.AI
**Authors:** Kale-ab Abebe Tessera, Andras Szecsenyi, Cameron Barker, Alexander Rutherford et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
As language models are increasingly deployed as autonomous agents, they must coordinate with others over long horizons in open-ended interactive tasks. Yet existing evaluations rarely test these demands together, instead emphasising single-agent tasks, short interactions, or highly structured multi-agent settings. We introduce $alem$, a JAX-based benchmark for open-ended multi-agent coordination built on Craftax-like dynamics. Alem embeds procedurally generated coordination tasks, soft specialisation, communication, and controllable coordination difficulty into a long-horizon survival world with exploration, crafting, trading, and combat. We evaluate $13$ modern LLMs zero-shot within homogeneous teams, with trained MARL agents as reference points. Current LLM agents remain far from solving alem, averaging only ~6% normalised return, but their failures are not uniform. On the hardest coordination setting, zero-shot Gemini-3.1-Pro-High approaches MARL agents trained for one billion steps, while GPT-5.4-High achieves strong base-task reward but much lower coordination reward. This contrast shows that individual task competence does not imply coordination competence. Ablations show that communication is the largest contributor to coordination, while memory and reasoning help when used to maintain multi-step plans. Overall, our results identify coordination as a distinct bottleneck for frontier LLM agents, separate from single-agent capabilities. Alem makes this bottleneck measurable and provides a controlled testbed for developing agents that communicate, allocate roles, and execute shared plans. Code is available at https://github.com/alem-world/alem-env.

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[multi-agent-systems|Multi-agent systems]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.08340v1)
