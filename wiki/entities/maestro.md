---
type: entity
entity_type: framework
aliases: [MAESTRO, Multi-Agent Environment Security Threat Risk and Outcome]
tags: [security, framework, standards, threat-modeling, agents]
created: 2026-06-23
updated: 2026-06-23
url: https://cloudsecurityalliance.org/blog/2025/02/06/agentic-ai-threat-modeling-framework-maestro
---

# MAESTRO

*A seven-layer threat-modeling method built for agentic AI — find where a specific multi-agent system breaks, layer by layer.*

## What it is
CSA's **M**ulti-**A**gent **E**nvironment, **S**ecurity, **T**hreat, **R**isk, and **O**utcome framework (Feb 2025). It models an agentic system as seven layers — **foundation models, data operations, agent frameworks, deployment infrastructure, evaluation & observability, security & compliance** (a cross-cutting/vertical concern), and the **agent ecosystem** — and walks threats *within* each layer and *across* layers. Its premise: security isn't one layer, it's a property each layer must hold, and cross-layer interactions are where agentic risk actually lives.

## Why it matters
[[owasp-agentic-top-10|OWASP]] is a checklist and [[mitre-atlas|ATLAS]] is a technique catalog; MAESTRO is the *method* you run against a concrete deployment to discover its specific failure points. Its layer model maps almost one-to-one onto the autonomy spectrum and onto the radar's own structure — foundation model, [[tool-use|tools]], [[agent-memory|memory]], [[agent-protocols|inter-agent protocols]], [[agent-evaluation|eval/observability]] — which makes it the natural scaffold for threat-modeling a real multi-agent build.

## Relationships
- authored by [[cloud-security-alliance]]
- complements [[nist-ai-rmf]], [[owasp-llm-top-10]], [[owasp-agentic-top-10]], [[mitre-atlas]]
- part of the [[security-standards]] layer for [[agent-security]], [[multi-agent-systems]]
- layers map to [[tool-use]], [[agent-memory]], [[agent-protocols]], [[agent-evaluation]]

## Cited by
<!-- Auto-maintained by the kg-curator skill. -->
