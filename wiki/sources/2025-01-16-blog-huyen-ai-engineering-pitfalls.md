---
type: source
source_type: blog
title: "Common pitfalls when building generative AI applications"
author: Chip Huyen
outlet: huyenchip.com
url: https://huyenchip.com/2025/01/16/ai-engineering-pitfalls.html
resource: https://huyenchip.com/2025/01/16/ai-engineering-pitfalls.html
date: 2025-01-16
stake: Author of *AI Engineering* (O'Reilly, 2025); advises teams building AI products — vendor-neutral. Now building in robotics
ingested: 2026-06-22
tags: [perspective, agentic-ai, agent-evaluation, llm-as-judge, tool-use]
---

# Common pitfalls when building generative AI applications

**Blog** · Chip Huyen (huyenchip.com) · 2025-01-16 · [link](https://huyenchip.com/2025/01/16/ai-engineering-pitfalls.html)

**The take (attributed):** Huyen argues the failures she sees in production gen-AI aren't model failures — they're **discipline failures**: reaching for gen AI (and agentic frameworks) when simpler tools win, mistaking a product problem for an AI problem, over-trusting demos, and dropping human evaluation in favor of [[llm-as-judge|AI judges]].

**Stake:** Field notes from advising teams + her book *AI Engineering*; no model/framework to sell. The throughline — "product + evaluation discipline beats shiny tooling" — is consistent with her vendor-neutral lane.

## Argument
Six pitfalls; the agent-relevant ones do the work here:
- **Start too complex (#3).** Her sharpest anti-over-engineering line: don't use "an **agentic framework when direct API calls work**," a vector DB when term-based retrieval works, or finetuning when prompting works. Early framework adoption *abstracts away* critical detail (hard to debug) and *injects* bugs — she "often find[s] typos in default prompts when reviewing a framework's codebase," and a silent framework prompt-update can change your app's behavior unexplained. Abstractions are good eventually, "but … as we're still in the early days of AI engineering, best practices are still evolving, we should be more vigilant." (Directly anti-premature-agent-framework.)
- **Over-index on early success (#4).** Demo ≠ product, with numbers: **LinkedIn** took 1 month to hit 80% of target experience and **+4 more months to pass 95%**; an ecommerce AI-sales-assistant startup found 0→80% took as long as 80→90%, citing **tool calling** ("hard for agents to differentiate similar tools"), the accuracy/latency tradeoff (more planning/self-correction = more nodes = more latency), and untestability (infinite query combos). Production roadblocks she names: reliability (10% of one team's API calls timed out; model swaps change behavior), compliance (copyright, privacy, data lineage), safety (abuse, offensive outputs).
- **Forgo human evaluation (#5).** Teams lean fully on **[[llm-as-judge|AI-as-a-judge]]** and drop humans — but judges aren't deterministic and "must be evaluated and iterated over time, just like all other AI applications." Best teams pair automated eval with **daily human eval of 30–1000 outputs**: to correlate human vs AI scores (divergence → suspect the judge), to understand real usage, and to catch behavior drift. "Staring at data for just 15 minutes usually gives me some insight that could save me hours." (Cites Greg Brockman on manual data inspection.)
- The product-vs-AI pitfalls (#1 use gen AI when you don't need it; #2 confuse 'bad product' with 'bad AI'; #6 crowdsource use cases) reinforce that "**the AI components … are similar; the differentiation is product**" — execs who crowdsource use cases get "a million text-to-SQL models, a million Slack bots, and a billion code plugins."

## Why it matters / where it cuts
This is the **field-evidence counterpart** to her "Agents" framework — and the radar's clearest practitioner voice for the *simplicity-first* side of [[debate-agents-vs-workflows]]: "agentic framework when direct API calls work" is a near-verbatim restatement of Anthropic's "find the simplest solution… this might mean not building agentic systems at all." Her insistence that **AI judges must themselves be validated against human eval** is a load-bearing caveat for [[agent-evaluation]] and [[llm-as-judge]] — the radar's arxiv layer keeps surfacing evaluator-bias and judge-gaming failures, and Huyen's "correlate daily with humans" is the practitioner mitigation. The compounding 80→95% gap is the same long-horizon reliability wall her Agents post quantifies (the 0.6%-over-100-steps math).

## Graph
- **Author:** [[chip-huyen]]
- **Concepts:** [[agentic-ai]] · [[agent-evaluation]] · [[llm-as-judge]] · [[tool-use]] · [[agent-reliability]]
- **Entities:** [[anthropic]] (echoes "Building Effective Agents" simplicity thesis)
- **Debate:** [[debate-agents-vs-workflows]] (ally of the simplicity / "simplest-that-works" camp)
- **Raw:** `raw/blogs/2025-01-16-chip-huyen-ai-engineering-pitfalls.md`
