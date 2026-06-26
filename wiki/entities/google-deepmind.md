---
type: entity
entity_type: org
aliases: [DeepMind, Google DeepMind, GDM]
tags: [agents, org, lab, foundation-models]
created: 2026-06-22
updated: 2026-06-22
url: https://deepmind.google/
---

# Google DeepMind

*Google's frontier AI lab — home of the [[gemini|Gemini]] models and a long line of agentic and world-model systems (AlphaGo → SIMA, Genie, Co-Scientist, AlphaEvolve).*

## What it is
The research-and-product AI lab inside Google that builds the [[gemini|Gemini]] family and a deep bench of agentic/embodied systems: the SIMA virtual-world agents, [[world-models|Genie]] world models, [[gemini|Gemini Robotics]], the AlphaEvolve coding agent, and the multi-agent **Co-Scientist**. Distinct from the broader [[google|Google]] entity in this radar (which tracks Google's open-model/infra footprint, e.g. Gemma + Vera Rubin) — DeepMind is the lab doing the agent and safety research itself.

## Why it matters
DeepMind is now publishing not just models but the *operating manual* for deploying agents safely at scale — its [[2026-06-18-blog-google-deepmind-securing-future-ai-agents|AI Control Roadmap]] (insider-threat modelling, supervisor-model monitoring, capability-gated controls, a million coding-agent trajectories analyzed) is the most concrete public account of how a frontier lab runs [[agent-security]]. On the build side, **Co-Scientist** is a flagship [[multi-agent-systems|multi-agent]] [[science-agents|science agent]] whose verification-heavy design is a reusable template. So what: watch DeepMind as both the agent-capability frontier (Gemini agentic features, embodied AI) and the de-facto author of enterprise agent-governance patterns.

## Relationships
- CEO [[demis-hassabis]]; chief scientist [[jeff-dean]]; mech-interp lead [[neel-nanda]]
- makes [[gemini]]
- part of [[google]]
- competes with [[anthropic]], [[openai]], [[meta-ai]]
- introduced [[agent-security]] AI Control Roadmap → [[2026-06-18-blog-google-deepmind-securing-future-ai-agents]]
- builds [[multi-agent-systems]] Co-Scientist → [[2026-05-19-blog-google-deepmind-co-scientist-multi-agent]]
- relates to [[world-models]] (Genie), [[embodied-agents]] (SIMA, Gemini Robotics), [[alphaevolve]]

## Perspective (blog-scanner)
- **"Securing the future of AI agents" (AI Control Roadmap)** (Shah & Flynn, Jun 2026): treat internal agents as insider threats; defense-in-depth + capability-gated monitoring; CoT-monitoring has a shelf life → [[2026-06-18-blog-google-deepmind-securing-future-ai-agents]]; feeds [[debate-prompt-injection-solvable]].
- **"Co-Scientist: A multi-agent AI partner to accelerate research"** (May 2026): supervisor-planner + generate/debate/evolve agents + Elo "idea tournament"; most compute spent on verification → [[2026-05-19-blog-google-deepmind-co-scientist-multi-agent]].

### Other agent-relevant 2025–26 posts (enumerated, not deep-captured)
- **SIMA 2** — "an agent that plays, reasons, and learns with you in virtual 3D worlds" ([[embodied-agents]]).
- **Genie 3** / Project Genie — generate and explore interactive worlds ([[world-models]]).
- **Gemini Robotics** — perceive, reason, use tools and interact ([[embodied-agents]]).
- **AlphaEvolve** — a Gemini-powered coding agent for designing advanced algorithms ([[coding-agents]], [[alphaevolve]]).
- **Investing in multi-agent AI safety research** (Jun 2026) — [[multi-agent-systems]], [[agent-security]].
- **Google Antigravity / Antigravity 2.0** — agentic development platform ([[coding-agents]]).
- **Gemini 3.5: frontier intelligence with action** (May 2026) — agentic Gemini ([[agentic-ai]]).
- **Gemini for Science** (I/O 2026) — agentic science tools ([[science-agents]]).
