---
type: source
source_type: blog
title: "Google's year in review: 8 areas with research breakthroughs in 2025"
author: Jeff Dean (with Demis Hassabis, James Manyika)
outlet: The Keyword (blog.google)
url: https://blog.google/innovation-and-ai/products/2025-research-breakthroughs/
resource: https://blog.google/innovation-and-ai/products/2025-research-breakthroughs/
date: 2025-12-23
stake: Google Chief Scientist — institutional book; this IS Google marketing its capability+infra year. Read the framing at a discount; treat the dated underlying releases as the facts.
ingested: 2026-06-22
tags: [perspective, agentic-ai, science-agents, reasoning-models, world-models, open-models, frontier-model-training]
---

# Google's year in review: 8 areas with research breakthroughs in 2025

**Blog** · Jeff Dean (lead author, with Demis Hassabis & James Manyika) · The Keyword / Google · 2025-12-23 · [link](https://blog.google/innovation-and-ai/products/2025-research-breakthroughs/)

**The take (attributed):** Dean and his co-authors argue **2025 was "the year of AI agents, reasoning and scientific discovery"** — the year AI's trajectory "shifted from a tool to a utility: from something people use to something they can put to work." It's Google's official capability-book summary, organized into 8 areas, and it is the closest thing to Dean's annual state-of-the-field statement.

**Stake:** This is a Google institutional post — Dean is Chief Scientist of the lab being celebrated. Every claim talks Google's book. The useful signal isn't the adjectives; it's *which* dated releases the chief scientist chose to anchor the year on, and the through-line he draws (agents + reasoning + science).

## Argument
- **Models / the Pareto trend.** The year ran Gemini 2.5 (March) → Gemini 3 + Gemini 3 Pro (Nov) → Gemini 3 Flash (Dec). They cite concrete marks: Gemini 3 Pro topped LMArena and hit breakthrough scores on [[gpqa|GPQA Diamond]] and Humanity's Last Exam, plus a new SOTA of **23.4% on MathArena Apex**. The post explicitly names the lab's signature efficiency thesis — *"the next generation's Flash model is better than the previous generation's Pro model"* — Gemini 3 Flash beats Gemini 2.5 Pro-scale "at a fraction of the price." On the open side, [[open-models|Gemma 3]] (and Gemma 3 270M) carry the "lightweight and open" line.
- **Products → agentic.** The framing is "tool to utility": software development "moving beyond tools that assist coding to... agentic systems that collaborate with developers" — Gemini 3 coding + **Google Antigravity** + **Jules** (an "asynchronous coding agent"). NotebookLM gains **Deep Research**; Search gains generative UI / AI Mode.
- **Science & math.** The post's center of gravity. AlphaFold's 5-year mark (3M+ researchers, 190+ countries); AlphaGenome, DeepSomatic, the **AI co-scientist** (Feb 2025), AlphaEvolve advancing theoretical CS; Gemini **Deep Think** taking gold-medal standard at both the **IMO** and the **ICPC World Finals**. Cell2Sentence-Scale 27B (a Gemma model) flagged as helping "discover a new potential cancer therapy pathway."
- **Computing / physical world.** Ironwood, "a new TPU built for the age of inference," designed using **AlphaChip**; a public energy-cost methodology for Gemini inference; Project Suncatcher (space-based AI infra); Quantum Echoes. Robotics + world models: Gemini Robotics 1.5 ("brings AI agents into the physical world") and **Genie 3** ("a new frontier for world models").
- **Global impact.** "State-of-the-art foundational models and agentic reasoning" applied to flood forecasting (2B+ people, 150 countries), WeatherNext 2 (8x faster), Earth AI / AlphaEarth, AMIE for disease management.
- **Safety & collaboration.** Gemini 3 framed as "our most secure model yet"; "a responsible path to AGI"; the **Frontier Safety Framework**; co-founding the **Agentic AI Foundation** (with MCP, goose, AGENTS.md) and shipping **MCP support for Google services** — i.e. Google publicly committing to agent interop standards. Plus the DOE national-labs "Genesis" science partnership.

## Why it matters / where it cuts
This is the single best one-document read on **where Google's chief scientist is pointing the whole book** going into 2026, and three threads matter for the exec: (1) **agents are now the product framing**, not a research curiosity — Antigravity/Jules/Deep Research + MCP-interop signal Google competing on the agentic stack, not just model quality; (2) the **Flash-beats-last-gen-Pro** efficiency curve is the explicit strategy (it's the [[2026-02-12-blog-dean-latent-space-pareto-frontier|Pareto-frontier]] thesis productized); (3) **AI-for-science is Google's differentiated bet** (co-scientist, AlphaEvolve, AlphaGenome, IMO/ICPC gold). Discount the "most secure model yet" language — it's marketing — but note the institutional move to bless agent interop standards (MCP, AAIF) as a real strategic signal.

## Graph
- **Author:** [[jeff-dean]]
- **Entities:** [[google]] · [[google-deepmind]] · [[gemini]]
- **Concepts:** [[agentic-ai]] · [[reasoning-models]] · [[science-agents]] · [[world-models]] · [[open-models]] · [[coding-agents]] · [[frontier-model-governance]]
- **Related:** [[mcp]] (Agentic AI Foundation / MCP-for-Google) · [[alphaevolve]] · [[multi-agent-systems]] (co-scientist)
- **Raw:** `raw/blogs/2025-12-23-dean-google-year-in-review-2025.md`
