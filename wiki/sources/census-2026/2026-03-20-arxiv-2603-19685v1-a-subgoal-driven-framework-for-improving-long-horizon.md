---
type: source
source_type: arxiv
title: "A Subgoal-driven Framework for Improving Long-Horizon LLM Agents"
authors: Taiyi Wang, Sian Gooding, Florian Hartmann, Oriana Riva et al.
url: https://arxiv.org/abs/2603.19685v1
date: 2026-03-20
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.AI
tags: [computer-use-agents, embodied-agents, agentic-rl, agent-memory, agent-evaluation, arxiv, auto-ingested]
---

# A Subgoal-driven Framework for Improving Long-Horizon LLM Agents

**arXiv:** [2603.19685v1](https://arxiv.org/abs/2603.19685v1) · 2026-03-20 · cs.AI
**Authors:** Taiyi Wang, Sian Gooding, Florian Hartmann, Oriana Riva et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Large language model (LLM)-based agents have emerged as powerful autonomous controllers for digital environments, including mobile interfaces, operating systems, and web browsers. Web navigation, for example, requires handling dynamic content and long sequences of actions, making it particularly challenging. Existing LLM-based agents struggle with long-horizon planning in two main ways. During online execution, they often lose track as new information arrives, lacking a clear and adaptive path toward the final goal. This issue is further exacerbated during reinforcement learning (RL) fine-tuning, where sparse and delayed rewards make it difficult for agents to identify which actions lead to success, preventing them from maintaining coherent reasoning over extended tasks. To address these challenges, we propose two contributions. First, we introduce an agent framework that leverages proprietary models for online planning through subgoal decomposition. Second, we present MiRA (Milestoning your Reinforcement Learning Enhanced Agent), an RL training framework that uses dense, milestone-based reward signals. The real-time planning mechanism improves proprietary models such as Gemini by approximately a 10% absolute increase in success rate (SR) on the WebArena-Lite benchmark. Meanwhile, applying MiRA to the open Gemma3-12B model increases its success rate from 6.4% to 43.0%. This performance surpasses proprietary systems such as GPT-4-Turbo (17.6%) and GPT-4o (13.9%), as well as the previous open-model state of the art, WebRL (38.4%). Overall, our findings demonstrate that combining explicit inference-time planning with milestone-based rewards significantly improves an agent's long-horizon capabilities, paving the way for more robust and general-purpose autonomous systems.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[embodied-agents|Embodied agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]]
- **Entities:** [[gpt-5]] · [[gemini]] · [[webarena]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.19685v1)
