---
type: source
source_type: blog
title: "Introducing AgentKit"
author: OpenAI
outlet: OpenAI news
url: https://openai.com/index/introducing-agentkit/
resource: https://openai.com/index/introducing-agentkit/
date: 2025-10-06
stake: Vendor platform launch (DevDay) — OpenAI shipping and marketing AgentKit (Agent Builder, Connector Registry, ChatKit), expanded Evals, and RFT. Customer metrics (Ramp 70%, Carlyle 50%/30%, Canva, LY Corp) are self-reported customer quotes, not independent measurements.
ingested: 2026-06-22
tags: [perspective, agentic-ai, multi-agent-systems, tool-use, agent-evaluation, agent-security, agent-protocols]
---

# Introducing AgentKit

**Blog** · OpenAI · 2025-10-06 · [link](https://openai.com/index/introducing-agentkit/)

**The take (attributed):** OpenAI argues that building agents is still too fragmented — orchestration without versioning, custom connectors, manual eval pipelines, weeks of frontend work — and pitches AgentKit as the end-to-end platform (visual builder + connectors + embeddable chat + evals + safety) that turns the [[agentic-ai|Agents SDK]] foundation into a productized workflow.

**Stake:** DevDay platform launch. The "build an agent in hours not quarters" customer metrics are OpenAI's logos quoting themselves. The strategic read is OpenAI moving up the stack from API primitives to a low-code agent platform — competing with the orchestration frameworks, not just other model labs.

## Argument
AgentKit bundles three new building blocks on top of the [[tool-use|Agents SDK / Responses API]] stack:
- **Agent Builder** — a visual canvas for creating and *versioning* [[multi-agent-systems|multi-agent]] workflows: drag-and-drop nodes, tool connections, custom guardrails, preview runs, inline eval config, templates. (This is OpenAI productizing the handoffs/guardrails model from its March 2025 SDK into a GUI.)
- **Connector Registry** — central admin control for how data and tools connect across ChatGPT and the API, with prebuilt connectors (Dropbox, Google Drive, SharePoint, Teams) and **third-party [[mcp|MCPs]]** — a notable ratification of MCP as the connector layer, which the March 2025 launch had sidestepped.
- **ChatKit** — embeddable, customizable chat-agent UI for your own product.

Plus an expanded **[[agent-evaluation|Evals]]** suite (Datasets, Trace grading, Automated prompt optimization, third-party model support) and reinforcement fine-tuning betas (Custom tool calls, Custom graders; RFT GA on [[openai-o3|o4-mini]], private beta for [[gpt-5|GPT-5]]).
On [[agent-security|safety]]: **Guardrails**, "an open-source, modular safety layer" that can mask/flag PII, detect jailbreaks, and apply other safeguards, usable standalone or via Python/JS.
Self-reported customer metrics: Ramp ("iteration cycles by 70%"), Carlyle ("development time… over 50%… accuracy 30%"), LY Corporation (multi-agent workflow "in less than two hours"), Canva ("over two weeks… in less than an hour"); plus Klarna and Clay as prior proof points.

## Why it matters / where it cuts
AgentKit is OpenAI's move from "here are agent APIs" to "here is the platform to build, version, connect, eval, and ship agents" — closing the loop the [[harness-engineering|harness]] and [[agent-evaluation|eval-tooling]] discourse kept flagging as the real bottleneck. So what: two signals matter. First, the inline **evals + trace grading + prompt optimization** is OpenAI conceding that the hard part of agents is measurement, not the model — aligned with the [[debate-evals-vs-frameworks|evals-vs-frameworks]] argument. Second, the **Connector Registry embracing third-party MCP** is OpenAI ratifying the open connector standard it earlier sidestepped — a meaningful consolidation of [[agent-protocols|the protocol layer]] around MCP. Read the productivity metrics as directional marketing; read the platform shape as the durable competitive move against LangGraph/CrewAI-style orchestration.

## Graph
- **Author:** [[openai]]
- **Concepts:** [[agentic-ai]] · [[multi-agent-systems]] · [[tool-use]] · [[agent-evaluation]] · [[agent-security]] · [[agent-protocols]]
- **Entities:** [[openai]] · [[mcp]] · [[gpt-5]] · [[openai-o3]]
- **Debate:** [[debate-evals-vs-frameworks]]
- **Raw:** `raw/blogs/2025-10-06-openai-introducing-agentkit.md`
