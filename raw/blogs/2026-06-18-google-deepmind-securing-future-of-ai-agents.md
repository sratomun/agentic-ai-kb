# Securing the future of AI agents (AI Control Roadmap)

Source: https://deepmind.google/blog/securing-the-future-of-ai-agents/
Authors: Rohin Shah and Four Flynn (research authors: Mary Phuong, Erik Jenner, Laurent Simon, Lewis Ho, Rohin Shah, Sebastian Farquhar, Scott Coull)
Date: June 18, 2026
Outlet: Google DeepMind blog (Responsibility & Safety)
Captured: 2026-06-22

---

How we're securing internal systems against increasingly capable and imperfectly aligned AI.

AI agents are transforming our relationship with technology. By autonomously executing complex tasks — from cyber defence to scientific discovery and product development — these systems are unlocking a new era of productivity. In the U.S alone, AI agents could create $2.9 trillion in economic value by 2030 (cites McKinsey).

As these agents become more capable, they also require more sophisticated safeguards. That's why we developed our **AI Control Roadmap**: a framework for building and managing the advanced AI we deploy within Google. This "defense-in-depth" approach goes beyond traditional model alignment, adding a crucial layer of system-level security that provides assurance even if alignment is imperfect.

## Understanding AI Control

Our approach starts with traditional safeguards like sandboxing, endpoint security, and prompt injection resistance. On top of this, the AI Control Roadmap uses model alignment (training AI to be inherently safe and helpful) as a primary defense, then adds a layer that treats internal agents as potentially misaligned, providing assurance even if alignment is imperfect.

Analogy: a driving instructor with dual controls — trusts the student but stays ready to take the wheel. The AI control system grants AI agents permissions based on their verified behavior, building trust through controlled, incremental access.

The roadmap focuses on three key areas:

1. **Novel threat-modelling framework for AI.** Treats untrusted AI agents as potential "insider threats" — similar to a potential rogue employee with office access. Builds on the industry-standard MITRE ATT&CK framework to break down potential attacks into smaller tactics and techniques, to track risks, spot bad behavior before it causes damage, and run drills.
2. **A plan to deploy AI control mitigations.**
   - Detection: Monitoring is the backbone. Uses other, trusted AI systems as "supervisors" to constantly review a working agent's reasoning, actions and plans.
   - Prevention and Response: If a supervisor sees the agent trying to do something harmful, it can step in to block the action before damage occurs.
3. **Constantly measure performance** across three metrics: coverage (fraction of traffic monitored), recall (fraction of misaligned behaviors caught), and time-to-response.

## Scaling security as AI gets smarter

Maps security protocols to measurable milestones in AI capabilities on two fronts:

- **Ability to evade detection:** Today we monitor a model's visible chain-of-thought. As models learn to hide reasoning — through *oversight awareness* (knowing they're monitored) or *opaque reasoning* (reasoning without visible text) — reading verbalized reasoning won't be enough; we'll need to analyze behavior and inspect inner workings. Detection levels D1-D4.
- **Ability for potential harm:** For low-risk reversible actions, review transcripts with a delay and remediate after the fact (asynchronous response). For high-risk actions (e.g. major cyber attacks), shift to real-time prevention, blocking harmful actions before execution (synchronous response). Prevention/Response levels R1-R3. The model's detection-evasion capability determines the Detection level; its attack-execution capability determines the Prevention and Response level.

## Analyzing a million agent trajectories to inform live monitoring

The team built an internal prototype of an asynchronous monitoring system that reviews coding agent trajectories and escalates findings for human review. Each flagged event is classified against the threat taxonomy. They have analyzed a million coding agent tasks, allowing them to move beyond simple keyword filtering to high-signal behavioral patterns. This was instrumental in building a live monitor for the **Gemini Spark agent**, responding in real-time to issues like unintentional data deletion.

Important note: the majority of flagged events do not stem from adversarial intent; instead, they often result from agent misinterpretation or overeagerness to achieve a user's goal (cites arxiv 2605.30322).

## Defending the agent ecosystem is a shared responsibility

The AI Control Roadmap is one element of a multilayered approach. DeepMind is also publishing a technical framework for policymakers, **'Three Layers of Agent Security'** — improving security at the level of individual agents; in multi-agent systems; and to empower cyber defenders and build resilience across the broader ecosystem.

Full technical report: AI Control Roadmap (PDF).
