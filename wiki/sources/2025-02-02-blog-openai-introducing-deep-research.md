---
type: source
source_type: blog
title: "Introducing deep research"
author: OpenAI
outlet: OpenAI news
url: https://openai.com/index/introducing-deep-research/
resource: https://openai.com/index/introducing-deep-research/
date: 2025-02-02
stake: Vendor product launch — OpenAI shipping and marketing deep research in ChatGPT, powered by a version of o3. HLE (26.6%) and GAIA SOTA figures are OpenAI's own evals; "research-analyst level" and "step toward AGI" are marketing framing.
ingested: 2026-06-22
tags: [perspective, agentic-ai, deep-research-agents, reasoning-models, tool-use, agent-evaluation]
---

# Introducing deep research

**Blog** · OpenAI · 2025-02-02 · [link](https://openai.com/index/introducing-deep-research/)

**The take (attributed):** OpenAI argues that an end-to-end-RL-trained agent that browses, runs Python, and cites sources can do multi-step web research "at the level of a research analyst" — accomplishing in tens of minutes what takes a human hours — and frames knowledge synthesis as a stepping stone toward AGI.

**Stake:** Product launch. The "research-analyst level" claim and the AGI framing are OpenAI marketing its own ChatGPT feature; the HLE and GAIA numbers are its own benchmark runs (and OpenAI notes it blocked leaked HLE answer sites). Treat the capability as real and notable, the magnitude claims at a discount.

## Argument
Deep research is a [[deep-research-agents|deep-research agent]] powered by a version of the (then-upcoming) [[openai-o3|o3]] model optimized for web browsing and data analysis. Per OpenAI it was trained with the same RL methods behind [[openai-o1|o1]] — end-to-end reinforcement learning on hard browsing and reasoning tasks — so it learns to plan a multi-step trajectory, backtrack, and react to information it encounters ([[agentic-rl|RL for agents]] applied to web research). It browses uploaded files, plots and iterates on graphs via Python, embeds images, and cites specific passages.
- **Humanity's Last Exam:** 26.6% with browsing + Python — OpenAI's reported new high (vs o1 9.1, o3-mini high 13.0 in its table).
- **[[gaia-benchmark|GAIA]]:** new SOTA topping the external leaderboard — pass@1 avg 67.36, cons@64 avg 72.57 (vs prior SOTA 63.64).
- **Internal expert-level tasks:** rated by domain experts to automate multiple hours of manual investigation; "the more the model browses and thinks about what it's browsing, the better it does."

OpenAI is candid on [[agent-reliability|limits]]: it can hallucinate or misinfer (lower rate than prior ChatGPT models per internal evals), struggles to separate authoritative info from rumor, and has weak confidence calibration. The Feb 3 addendum rates the early o3 powering it as Medium risk under the Preparedness Framework.

## Why it matters / where it cuts
This is the post that made "deep research" a product category — every other lab now ships a deep-research mode, and it set the template ([[reasoning-models|reasoning model]] + browser + Python + citations, trained by RL on real tasks). So what: this is the canonical reference for what an autonomous research agent can and can't do, with OpenAI's own reliability caveats (confidence calibration, rumor-vs-fact) usefully on the record. Note the trajectory in the update log — by Feb 2026 deep research connects to any [[mcp|MCP]] or app and can restrict to trusted sites, closing the "can't reach my internal sources" gap that limited the launch version. It pairs in OpenAI's own framing with Operator/ChatGPT agent: research (read) + action (write) as the two halves of an agentic ChatGPT.

## Graph
- **Author:** [[openai]]
- **Concepts:** [[agentic-ai]] · [[deep-research-agents]] · [[reasoning-models]] · [[tool-use]] · [[agent-evaluation]] · [[agentic-rl]]
- **Entities:** [[openai]] · [[openai-o3]] · [[openai-o1]] · [[gaia-benchmark]]
- **Raw:** `raw/blogs/2025-02-02-openai-introducing-deep-research.md`
