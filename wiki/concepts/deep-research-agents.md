---
type: concept
tags: [agents, deep-research, retrieval, web]
created: 2026-06-22
updated: 2026-06-22
census_count: 119
kind: domain
---

# Deep-research agents

*Agents that autonomously turn a question into a sourced report — iterative web search, browsing, synthesis, and long-form writing.*

## What it is
The product pattern behind OpenAI/Google "Deep Research" and a wave of open clones: an agent that plans a research task, searches and browses the live web, reconciles sources, and drafts an analyst-grade, citation-rich report — compressing hours of desk research into minutes. It sits at the intersection of [[agentic-rag]], [[tool-use]] (search/browse), and [[computer-use-agents]].

## Why it matters
The highest-visibility consumer *and* enterprise agent pattern of 2025 — and the cleanest template for knowledge-work automation, which is your domain. It's also where the field learned that **end-to-end RL on the real web** beats prompt-engineered pipelines, a lesson now propagating to other verticals.

## What the evidence shows
**2025 foundations.** The category went from prompt-glue to *trained*. **Search-o1** first folded an agentic-RAG step (plus a Reason-in-Documents refiner) into o1-style reasoning to fix knowledge-insufficiency (→ [[2025-01-09-arxiv-2501-05366v1-search-o1-agentic-search-enhanced-large-reasoning-models]]). **WebThinker** trained the loop with iterative online DPO and **beat strong proprietary systems on GPQA/GAIA/WebWalkerQA/HLE** (→ [[2025-04-30-arxiv-2504-21776v2-webthinker-empowering-large-reasoning-models-with-deep-research]]). **DeepResearcher** was the first end-to-end RL framework trained against *authentic* live web search (not a sandboxed RAG), improving up to **+28%** (→ [[2025-04-04-arxiv-2504-03160v4-deepresearcher-scaling-deep-research-via-reinforcement-learning-in]]). Evaluation kept pace — **BrowseComp** (1,266 hard browsing tasks → [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing]]) and **DeepResearch Bench** (100 PhD-level tasks → [[2025-06-13-arxiv-2506-11763v1-deepresearch-bench-a-comprehensive-benchmark-for-deep-research]]) — alongside WebSailor and WebDancer.

## Relationships
- canonical launch (OpenAI) → [[2025-02-02-blog-openai-introducing-deep-research]]; Anthropic multi-agent research → [[2025-06-13-blog-anthropic-multi-agent-research-system]]
- builds on [[agentic-rag]], [[tool-use]], [[computer-use-agents]]
- trained via [[agentic-rl]]; powered by [[reasoning-models]]
- evaluated in [[agent-evaluation]] (BrowseComp, DeepResearch Bench)
- a form of [[agentic-ai]]

## Key 2025 papers (citation-ranked)
- **441** · [[2025-04-16-arxiv-2504-12516v1-browsecomp-a-simple-yet-challenging-benchmark-for-browsing|BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents]]
- **429** · [[2025-01-09-arxiv-2501-05366v1-search-o1-agentic-search-enhanced-large-reasoning-models|Search-o1: Agentic Search-Enhanced Large Reasoning Models]]
- **279** · [[2025-04-30-arxiv-2504-21776v2-webthinker-empowering-large-reasoning-models-with-deep-research|WebThinker: Empowering Large Reasoning Models with Deep Research Capability]]
- **220** · [[2025-04-04-arxiv-2504-03160v4-deepresearcher-scaling-deep-research-via-reinforcement-learning-in|DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world ...]]
- **170** · [[2025-07-03-arxiv-2507-02592v1-websailor-navigating-super-human-reasoning-for-web-agent|WebSailor: Navigating Super-human Reasoning for Web Agent]]
- **168** · [[2025-06-13-arxiv-2506-11763v1-deepresearch-bench-a-comprehensive-benchmark-for-deep-research|DeepResearch Bench: A Comprehensive Benchmark for Deep Research Agents]]
- **147** · [[2025-05-28-arxiv-2505-22648v3-webdancer-towards-autonomous-information-seeking-agency|WebDancer: Towards Autonomous Information Seeking Agency]]
