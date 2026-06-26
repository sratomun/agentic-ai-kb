---
type: entity
entity_type: framework
aliases: [MITRE ATLAS, ATLAS, Adversarial Threat Landscape for Artificial-Intelligence Systems]
tags: [security, framework, standards, threat-intel]
created: 2026-06-23
updated: 2026-06-23
url: https://atlas.mitre.org/
---

# MITRE ATLAS

*ATT&CK for AI — a living matrix of adversary tactics and techniques against AI systems, grounded in real red-team cases.*

## What it is
The Adversarial Threat Landscape for Artificial-Intelligence Systems: a knowledge base of **16 tactics** (adversary goals like reconnaissance, ML model access, poisoning, evasion, exfiltration, impact) and **84 techniques** beneath them, plus real-world case studies. It mirrors the structure of MITRE ATT&CK and covers the full AI lifecycle — data collection and training through deployment and operation — including jailbreaks, training-data poisoning, model extraction, and prompt-injection techniques.

## Why it matters
ATLAS is the framework that lets an existing SOC reason about AI attacks in the language it already uses. Tactics-and-techniques is how threat-intel, detection engineering, and red teams already work via ATT&CK, so ATLAS is the lowest-friction on-ramp for a cyber team to start covering agentic threats — and the natural backbone for red-team test plans and detection coverage maps. Complements the others: [[owasp-agentic-top-10|OWASP]] tells you *what* risks rank, ATLAS tells you *how* adversaries get there.

## Relationships
- maintained by [[mitre]] (sibling of ATT&CK)
- complements [[nist-ai-rmf]], [[owasp-llm-top-10]], [[owasp-agentic-top-10]], [[maestro]]
- part of the [[security-standards]] layer for [[agent-security]]
- techniques cover radar attack classes: prompt injection, poisoning, [[tool-description-poisoning]], model extraction

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
