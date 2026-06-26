---
type: concept
tags: [agents, computer-use, gui, web]
created: 2026-06-21
updated: 2026-06-22
census_count: 323
kind: domain
---

# Computer-use & GUI agents

*Agents that operate software the way a person does — clicking, typing, navigating GUIs, browsers, and operating systems.*

## What it is
Agents that act in the *digital world* through the interface a human uses, not through APIs: perceiving a screen, grounding an instruction to a UI element, and executing multi-step tasks across browsers, desktops, and mobile (the CUA stack + GUI grounding). Evaluated on [[osworld]], [[webarena]], [[androidworld]], [[appworld]].

## Why it matters
Strategically the highest-leverage agent category for knowledge work: if an agent can drive arbitrary software, the addressable surface is *everything on a screen* — no integration, no API required. This is the category behind the OS-level platform plays (Microsoft, Anthropic computer use) and the one whose progress most directly threatens or augments desk work.

## What the evidence shows
**2025 foundations.** The breakthrough was going **end-to-end native** instead of wrapping a frontier model in prompts. **UI-TARS** is a single GUI model that outperforms GPT-4o-plus-scaffolding frameworks and set SOTA across 10+ GUI benchmarks including OSWorld (→ [[2025-01-21-arxiv-2501-12326v1-ui-tars-pioneering-automated-gui-interaction-with-native]]). The other half was **RL for GUI**: GUI-R1 used GRPO-style rule-based rewards to beat OS-Atlas across 8 benchmarks on 3 platforms using only ~0.13M training samples — efficiency, not scale (→ [[2025-04-14-arxiv-2504-10458v4-gui-r1-a-generalist-r1-style-vision-language]]). Evaluation hardened in parallel: **BrowseComp** (1,266 hard multi-hop browsing tasks → [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing]]) and **ScreenSpot-Pro** (high-resolution *professional* GUI grounding, where small targets break models → [[2025-04-04-arxiv-2504-07981v1-screenspot-pro-gui-grounding-for-professional-high-resolution]]). Web agents (WebSailor, WebWalker) and the Planner/Executor split ([[2025-03-12-arxiv-2503-09572v3-plan-and-act-improving-planning-of-agents-for|Plan-and-Act]]) round out the year.
- The 2025→26 bridge: web computer-use is the engine of [[deep-research-agents]]; the model class is [[vla]].

## Includes (sub-themes folded here)
Folds in: **GUI grounding** (ScreenSpot, GUI-R1, element localization — ~405 papers), browser/web agents, and OS/mobile-device control.

## Relationships
- OpenAI Operator/CUA + ChatGPT agent → [[2025-07-17-blog-openai-introducing-chatgpt-agent]]
- related 2025 theme: [[deep-research-agents]]; model class [[vla]]
- benchmarks: [[osworld]], [[webarena]], [[androidworld]], [[appworld]]
- relates to [[agent-skills]] (CUA stack), [[tool-use]]
- platform context: [[windows-365-for-agents]]
- a form of [[agentic-ai]]
- on-device variant: [[on-device-agents]] (local GUI/mobile agents)

## Key 2025 papers (citation-ranked)
- **464** · [[2025-01-21-arxiv-2501-12326v1-ui-tars-pioneering-automated-gui-interaction-with-native|UI-TARS: Pioneering Automated GUI Interaction with Native Agents]]
- **441** · [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing|BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents]]
- **222** · [[2025-04-04-arxiv-2504-07981v1-screenspot-pro-gui-grounding-for-professional-high-resolution|ScreenSpot-Pro: GUI Grounding for Professional High-Resolution Computer Use]]
- **218** · [[2025-04-14-arxiv-2504-10458v4-gui-r1-a-generalist-r1-style-vision-language|GUI-R1 : A Generalist R1-Style Vision-Language Action Model For GUI Agents]]
- **170** · [[2025-07-03-arxiv-2507-02592v1-websailor-navigating-super-human-reasoning-for-web-agent|WebSailor: Navigating Super-human Reasoning for Web Agent]]
- **162** · [[2025-03-12-arxiv-2503-09572v3-plan-and-act-improving-planning-of-agents-for|Plan-and-Act: Improving Planning of Agents for Long-Horizon Tasks]]
- **149** · [[2025-02-18-arxiv-2502-13130v1-magma-a-foundation-model-for-multimodal-ai-agents|Magma: A Foundation Model for Multimodal AI Agents]]
- **146** · [[2025-01-13-arxiv-2501-07572v3-webwalker-benchmarking-llms-in-web-traversal|WebWalker: Benchmarking LLMs in Web Traversal]]
