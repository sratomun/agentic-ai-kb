# Introducing AgentKit

Source: https://openai.com/index/introducing-agentkit/
Author: OpenAI
Date: October 6, 2025 (DevDay)
Category: Product
Captured: 2026-06-22
Note: the slug /index/agentkit/ did not resolve; the working/canonical URL is /index/introducing-agentkit/.
Vendor stake: OpenAI launching/marketing its own agent-building platform. Customer metrics (Ramp 70%, Carlyle 50%/30%, etc.) are self-reported customer quotes.

---

Today we're launching AgentKit, a complete set of tools for developers and enterprises to build, deploy, and optimize agents.

OpenAI frames AgentKit as a response to fragmented agent-building tooling — "complex orchestration with no versioning, custom connectors, manual eval pipelines, prompt tuning, and weeks of frontend work before launch."

## Core building blocks
- **Agent Builder:** a visual canvas for creating and versioning multi-agent workflows. Drag-and-drop nodes, tool connections, custom guardrails, preview runs, inline eval configuration, full versioning. Start blank or from prebuilt templates.
- **Connector Registry:** a central place for admins to manage how data and tools connect across OpenAI products. Consolidates sources across ChatGPT and the API; includes pre-built connectors (Dropbox, Google Drive, SharePoint, Microsoft Teams) and third-party MCPs.
- **ChatKit:** a toolkit for embedding customizable chat-based agent experiences in your product.

## Evals expansion
Four new capabilities: Datasets, Trace grading, Automated prompt optimization, and Third-party model support. Two new reinforcement fine-tuning (RFT) beta features: Custom tool calls and Custom graders. RFT is GA on OpenAI o4-mini and in private beta for GPT-5.

## Safety
Guardrails: "an open-source, modular safety layer" in Agent Builder that can "mask or flag PII, detect jailbreaks, and apply other safeguards." Deployable standalone or via Python/JavaScript libraries.

## Customers / metrics (self-reported)
- Ramp: built a buyer agent in hours, "slashing iteration cycles by 70%" — "an agent live in two sprints rather than two quarters."
- LY Corporation: built and ran a multi-agentic workflow "in less than two hours."
- Carlyle: "cut development time on our multi-agent due diligence framework by over 50%, and increased agent accuracy 30%."
- Canva: "saved over two weeks of time... integrated it in less than an hour" (support agent via ChatKit).
- Earlier proof points cited: Klarna (support agent handles two-thirds of all tickets); Clay (10x'ed growth with a sales agent).
- Other named logos: HubSpot, LegalOn, Albertsons, Actively, Evernote, Taboola, Rippling, Box, Bain & Company.

## Availability / pricing
ChatKit and the new Evals capabilities are GA to all developers. Agent Builder is in beta. Connector Registry is beginning beta rollout to some API, ChatGPT Enterprise and Edu customers with a Global Admin Console. All tools included with standard API model pricing. A standalone Workflows API and ChatGPT agent deployment options planned soon.

Tags: Product · DevDay · 2025
