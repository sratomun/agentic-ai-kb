---
type: concept
tags: [security, governance, standards, agents]
created: 2026-06-23
updated: 2026-06-23
source_count: 4
kind: crosscutting
---

# Security standards & frameworks

*The reference layer that turns scattered agent-security research into something a cyber team can govern, test, and audit against — four complementary frameworks, not competitors.*

## What it is
The authoritative scaffolding for AI and agent security: [[nist-ai-rmf|NIST AI RMF]] (risk management), [[owasp-llm-top-10|OWASP LLM Top 10]] + [[owasp-agentic-top-10|OWASP Top 10 for Agentic Applications]] (vulnerability checklists), [[mitre-atlas|MITRE ATLAS]] (adversary tactics & techniques), and [[maestro|CSA MAESTRO]] (layered threat modeling). They answer different questions and are meant to be stacked, not chosen between. The research-heavy [[agent-security]] hub is the *evidence*; this is the *map* that organizes it.

## Why it matters
Most agent-security material — including this radar's own — is a pile of attacks and defenses. These frameworks are what make it legible to a board, an auditor, or a SOC. The four divide the labor cleanly:

- **[[nist-ai-rmf|NIST]] — govern.** Govern / Map / Measure / Manage + a GenAI Profile (AI 600-1) naming 12 risk categories. Answers *who owns this risk and how do we show we manage it.* The compliance and accountability anchor.
- **[[owasp-llm-top-10|OWASP]] — enumerate.** Ranked checklists: LLM01–LLM10 for apps (prompt injection #1, Excessive Agency the bridge), ASI01–ASI10 + the T1–T15 taxonomy for agents (goal hijack, tool misuse, memory poisoning, rogue agents). Answers *what specifically to look for.*
- **[[mitre-atlas|MITRE ATLAS]] — attack.** 16 tactics / 84 techniques, ATT&CK-shaped, real cases. Answers *how adversaries actually get there* — the language a SOC already speaks.
- **[[maestro|CSA MAESTRO]] — model.** Seven layers (foundation model → data → frameworks → infra → eval → orchestration → ecosystem). Answers *where in this specific system does it break.*

EU AI Act and the emerging US federal posture (→ [[frontier-model-governance]], [[governance-gap]]) sit above these as compliance obligations, not threat frameworks.

## The autonomy spectrum (why holism matters)
Attack surface grows with autonomy, and the frameworks pick up the slack as you climb:

- **Raw LLM call** (no tools, no memory) — blast radius is a bad *output*. Surface: prompt injection, info disclosure, system-prompt leakage, confabulation, unbounded consumption. Covered by [[owasp-llm-top-10|LLM Top 10]] + [[nist-ai-rmf|NIST GenAI Profile]].
- **Single-turn tool agent** — the model can now *act*, once. Adds Excessive Agency, tool misuse, [[tool-description-poisoning|tool-description poisoning]], over-privileged tool selection, identity/privilege abuse, the lethal trifecta. [[owasp-agentic-top-10|Agentic Top 10]] ASI02/ASI03 + [[mitre-atlas|ATLAS]] techniques.
- **Autonomous / multi-agent** — loops, memory, planning, peers. Surface explodes: goal hijack, memory & context poisoning, cascading failures, insecure inter-agent comms, rogue agents, economic DoS, deceptive/misaligned behavior. [[owasp-agentic-top-10|Agentic Top 10]] in full + [[maestro|MAESTRO]] cross-layer modeling.

The radar's evidence maps onto every tier — see [[agent-security]] for the research backing (CaMeL, Sovereign Execution Brokers, [[tool-description-poisoning|TDP]], MemoryGraft, agentic misalignment, economic DoS).

## Relationships
- frameworks: [[nist-ai-rmf]], [[owasp-llm-top-10]], [[owasp-agentic-top-10]], [[mitre-atlas]], [[maestro]]
- bodies: [[nist]], [[owasp]], [[mitre]], [[cloud-security-alliance]]
- research mirror: [[agent-security]] (the evidence these frameworks organize)
- enterprise side: [[governance-gap]], [[frontier-model-governance]]
- attack classes: [[tool-description-poisoning]]; surfaces in [[tool-use]], [[agent-memory]], [[agent-protocols]], [[multi-agent-systems]]
- perspective: [[simon-willison]], [[debate-prompt-injection-solvable]]
