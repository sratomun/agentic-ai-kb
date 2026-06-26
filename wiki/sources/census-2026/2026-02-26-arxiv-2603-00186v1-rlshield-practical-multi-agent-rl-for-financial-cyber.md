---
type: source
source_type: arxiv
title: "RLShield: Practical Multi-Agent RL for Financial Cyber Defense with Attack-Surface MDPs and Real-Time Response Orchestration"
authors: Srikumar Nayak
url: https://arxiv.org/abs/2603.00186v1
date: 2026-02-26
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CR
tags: [finance-agents, agent-reliability, agentic-rl, agent-security, multi-agent-systems, arxiv, auto-ingested]
---

# RLShield: Practical Multi-Agent RL for Financial Cyber Defense with Attack-Surface MDPs and Real-Time Response Orchestration

**arXiv:** [2603.00186v1](https://arxiv.org/abs/2603.00186v1) · 2026-02-26 · cs.CR
**Authors:** Srikumar Nayak

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Financial systems run nonstop and must stay reliable even during cyber incidents. Modern attacks move across many services (apps, APIs, identity, payment rails), so defenders must make a sequence of actions under time pressure. Most security tools still use fixed rules or static playbooks, which can be slow to adapt when the attacker changes behavior. Reinforcement learning (RL) is a good fit for sequential decisions, but much of the RL-in-finance literature targets trading and does not model real cyber response limits such as action cost, service disruption, and defender coordination across many assets. This paper proposes RLShield, a practical multi-agent RL pipeline for financial cyber defense. We model the enterprise attack surface as a Markov decision process (MDP) where states summarize alerts, asset exposure, and service health, and actions represent real response steps (e.g., isolate a host, rotate credentials, ratelimit an API, block an account, or trigger recovery). RLShield learns coordinated policies across multiple agents (assets or service groups) and optimizes a risk-sensitive objective that balances containment speed, business disruption, and response cost. We also include a game-aware evaluation that tests policies against adaptive attackers and reports operational outcomes, not only reward. Experiments show that RLShield reduces time-to-containment and residual exposure while keeping disruption within a fixed response budget, outperforming static rule baselines and single-agent RL under the same constraints. These results suggest that multi-agent, cost-aware RL can provide a deployable layer for automated response in financial security operations.

## Graph
- **Concepts:** [[finance-agents|Finance agents]] · [[agent-reliability|Agent reliability]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2603.00186v1)
