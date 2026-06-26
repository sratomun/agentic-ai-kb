---
type: source
source_type: arxiv
title: "HearthNet: Edge Multi-Agent Orchestration for Smart Homes"
authors: Zhonghao Zhan, Krinos Li, Yefan Zhang, Hamed Haddadi
url: https://arxiv.org/abs/2604.09618v2
date: 2026-03-16
ingested: 2026-06-21
depth: abstract
auto: true
score: 19
primary: cs.DC
tags: [computer-use-agents, multi-agent-systems, arxiv, auto-ingested]
---

# HearthNet: Edge Multi-Agent Orchestration for Smart Homes

**arXiv:** [2604.09618v2](https://arxiv.org/abs/2604.09618v2) · 2026-03-16 · cs.DC
**Authors:** Zhonghao Zhan, Krinos Li, Yefan Zhang, Hamed Haddadi

> Auto-ingested from abstract (not full-text). Concept/entity links are keyword-derived.

## Abstract
Smart-home users increasingly want to control their homes in natural language rather than assemble rules, dashboards, and API integrations by hand. At the same time, real deployments are brittle: devices fail, integrations break, and recoveries often require manual intervention. Existing agent toolkits are effective for session-scoped delegation, but smart-home control operates under a different scenario: it is persistent, event-driven, failure-prone, and tied to physical devices with no shared context window. We present HearthNet, an edge multi-agent orchestration system for smart homes. HearthNet deploys a small set of persistent, role-specialized LLM agents at the home hub, where they coordinate through MQTT, Git-backed shared state, and root-issued actuation leases to govern heterogeneous devices through thin adapters. This design externalizes context, preserves execution history, and separates planning, verification, authorization, and actuation across explicit boundaries. Our current prototype runs on commodity edge hardware and Android devices; it keeps orchestration, state management, and device control on-premise while using hosted LLM APIs for inference. We demonstrate the system through three live scenarios: intent-driven multi-agent coordination from ambiguous natural language, conflict resolution with timeline-based tracing, and rejection of stale or unauthorized commands before device actuation.

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[multi-agent-systems|Multi-agent systems]]
- **Census record:** `raw/arxiv/2026-census/census-2026.jsonl` (id 2604.09618v2)
