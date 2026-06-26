---
type: entity
entity_type: org
aliases: [OWASP, OWASP GenAI Security Project, Open Worldwide Application Security Project]
tags: [security, org, standards]
created: 2026-06-23
updated: 2026-06-23
url: https://genai.owasp.org/
---

# OWASP

*The application-security community that ships the field's working vulnerability checklists — including the [[owasp-llm-top-10|LLM Top 10]] and the [[owasp-agentic-top-10|Top 10 for Agentic Applications]].*

## What it is
The Open Worldwide Application Security Project, a nonprofit whose **GenAI Security Project** produces the most-referenced practitioner artifacts for AI risk: the [[owasp-llm-top-10|OWASP Top 10 for LLM Applications]], the **Agentic AI – Threats and Mitigations** taxonomy (15 threats, T1–T15), and the [[owasp-agentic-top-10|OWASP Top 10 for Agentic Applications]] (ASI01–ASI10, Dec 2025). Community-driven and fast-moving — the opposite end of the spectrum from NIST's deliberate process.

## Why it matters
OWASP is the *vulnerability-enumeration* anchor of the [[security-standards|standards layer]] — concrete, checklist-shaped, and the lingua franca AppSec teams already speak. AWS and Microsoft now embed the agentic taxonomy in their own guidance, so OWASP codes are becoming the shared vocabulary for agent risk. The codes map directly onto the radar's own evidence: [[tool-description-poisoning|TDP]] sits under supply-chain/tool-misuse, [[2026-06-18-arxiv-2606-20023v1-over-privileged-tool-selection|over-privileged tool selection]] under Excessive Agency / Identity & Privilege Abuse.

## Relationships
- authored [[owasp-llm-top-10]], [[owasp-agentic-top-10]]
- complements [[nist]] (risk management), [[mitre]] (attack taxonomy), [[cloud-security-alliance]] (threat modeling)
- part of the [[security-standards]] layer for [[agent-security]]
- catalogs attack classes incl. [[tool-description-poisoning]], prompt injection (cf. [[simon-willison]], [[debate-prompt-injection-solvable]])
- relates to [[mcp]] (tool/supply-chain surface), [[agent-skills]] (supply chain)

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
