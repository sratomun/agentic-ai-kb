---
type: source
source_type: arxiv
title: "Agentra: A Supervisable Multi-Agent Framework for Enterprise Intrusion Response"
authors: Raj Patel, Shaswata Mitra, Michele Guida, Stefano Iannucci et al.
url: https://arxiv.org/abs/2606.18325v2
date: 2026-06-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 16
primary: cs.CR
tags: [knowledge-graph, agent-security, multi-agent-systems, governance-gap, arxiv, auto-ingested]
---

# Agentra: A Supervisable Multi-Agent Framework for Enterprise Intrusion Response

**arXiv:** [2606.18325v2](https://arxiv.org/abs/2606.18325v2) · 2026-06-16 · cs.CR
**Authors:** Raj Patel, Shaswata Mitra, Michele Guida, Stefano Iannucci et al.

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Enterprise intrusion response still depends on static playbooks and analyst-driven triage, creating delay between alert generation and containment. We present Agentra, a supervisable multi-agent Intrusion Response System (IRS) framework that converts alerts from IDS, EDR, and XDR platforms into structured incident response plans grounded in MITRE ATT&CK, MITRE D3FEND, and NIST CSF 2.0. Agentra decomposes response reasoning across role-scoped agents, validates proposed plans through a bounded Planner--Validator review loop, screens retrieved threat intelligence through a Moderator security gateway, gates actions through an Action Catalog and risk score, and records decisions in an append-only audit log. We evaluate Agentra against a static OASIS CACAO v2.0 cyber-playbook baseline on a 120-event corpus drawn from ThreatHunter-Playbook, Splunk BOTSv3, and DARPA OpTC. The strongest configuration improves FP-aware IRS F1 from 0.61 to 0.84 and restores the projected harmful-action rate to the static baseline level of 0.0% after Planner-only configurations introduce unsafe overreaction. These results indicate that multi-agent response planning can improve ontology-grounded IRS coverage while preserving analyst approval and auditability.

## Graph
- **Concepts:** [[knowledge-graph|Knowledge graphs]] · [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]] · [[governance-gap|Governance gap]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2606.18325v2)
