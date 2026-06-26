---
type: source
source_type: arxiv
title: "Enhancing Cloud Network Resilience via a Robust LLM-Empowered Multi-Agent Reinforcement Learning Framework"
authors: Yixiao Peng, Hao Hu, Feiyang Li, Xinye Cao et al.
url: https://arxiv.org/abs/2601.07122v2
date: 2026-01-12
ingested: 2026-06-21
depth: abstract
auto: true
score: 17
primary: cs.CR
tags: [human-agent-interaction, agent-reliability, agentic-rl, agent-security, agent-memory, arxiv, auto-ingested]
---

# Enhancing Cloud Network Resilience via a Robust LLM-Empowered Multi-Agent Reinforcement Learning Framework

**arXiv:** [2601.07122v2](https://arxiv.org/abs/2601.07122v2) · 2026-01-12 · cs.CR
**Authors:** Yixiao Peng, Hao Hu, Feiyang Li, Xinye Cao et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
While virtualization and resource pooling empower cloud networks with structural flexibility and elastic scalability, they inevitably expand the attack surface and challenge cyber resilience. Reinforcement Learning (RL)-based defense strategies have been developed to optimize resource deployment and isolation policies under adversarial conditions, aiming to enhance system resilience by maintaining and restoring network availability. However, existing approaches lack robustness as they require retraining to adapt to dynamic changes in network structure, node scale, attack strategies, and attack intensity. Furthermore, the lack of Human-in-the-Loop (HITL) support limits interpretability and flexibility. To address these limitations, we propose CyberOps-Bots, a hierarchical multi-agent reinforcement learning framework empowered by Large Language Models (LLMs). Inspired by MITRE ATT&CK's Tactics-Techniques model, CyberOps-Bots features a two-layer architecture: (1) An upper-level LLM agent with four modules--ReAct planning, IPDRR-based perception, long-short term memory, and action/tool integration--performs global awareness, human intent recognition, and tactical planning; (2) Lower-level RL agents, developed via heterogeneous separated pre-training, execute atomic defense actions within localized network regions. This synergy preserves LLM adaptability and interpretability while ensuring reliable RL execution. Experiments on real cloud datasets show that, compared to state-of-the-art algorithms, CyberOps-Bots maintains network availability 68.5% higher and achieves a 34.7% jumpstart performance gain when shifting the scenarios without retraining. To our knowledge, this is the first study to establish a robust LLM-RL framework with HITL support for cloud defense.

## Graph
- **Concepts:** [[human-agent-interaction|Human-agent interaction]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agent-memory|Agent memory]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2601.07122v2)
