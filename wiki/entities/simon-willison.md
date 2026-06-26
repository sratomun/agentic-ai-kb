---
type: entity
entity_type: person
aliases: [simonw]
tags: [agents, person]
affiliation: "Independent — writes daily at simonwillison.net; co-creator of Django, creator of Datasette/LLM (CLI); creator of the open-source `llm` Python library"
stake: Independent practitioner/educator — no model, lab, or framework to sell; revenue is a small newsletter/sponsorships. The field's reference-grade *disinterested* voice on agent security.
url: https://simonwillison.net/
created: 2026-06-22
updated: 2026-06-22
---

# Simon Willison

*Independent developer and the field's most prolific working-engineer LLM blogger — coined "prompt injection" (2022) and "the lethal trifecta" (2025), and is the clearest practitioner voice on agent security, coding agents, and what's actually useful vs. hype.*

## Who they are
Co-creator of the **Django** web framework and creator of **Datasette** and the **`llm`** CLI/Python library; now one of the most-read independent writers on practical LLM/agent engineering and security, posting daily at simonwillison.net (a mix of substantive original essays and a heavy link-blog). He writes from the **hands-on practitioner** lens — he ships tools with these models every day and reports what breaks. He coined "prompt injection" in 2022 and "the lethal trifecta" in 2025, framings that the major labs (Meta, Google, Anthropic, OpenAI) now cite back.

**Stake:** **Largely independent** — no model, lab, framework, or agent product to sell; income is a small newsletter plus sponsorships. That disinterest is exactly why his security warnings carry across the field: he has no book to talk. The one bias to weight: he's a *power-user enthusiast* of coding agents (runs them in unrestricted "YOLO mode" himself), so his optimism on agent **utility** is that of an early-adopter virtuoso — read his "this is incredibly useful" through that lens, while his security **skepticism** is, if anything, against his own enjoyment.

## What they argue (recurring stances)
- **Prompt injection is structural and unsolved** — LLMs "follow instructions in content" and can't reliably tell *whose* instructions to trust; "anyone who can get their tokens into your context should be considered to have full control over what your agent does next." (See [[2025-06-16-blog-willison-lethal-trifecta|lethal trifecta]].)
- **The [[tool-description-poisoning|lethal trifecta]]** = private-data access + exposure to untrusted content + ability to externally communicate. Combine all three and exfiltration is near-certain. By late 2025 he endorses Meta's **"Agents Rule of Two"** as a strictly better operational rule (it adds "change state" to capture non-exfiltration harms). ([[2025-11-02-blog-willison-new-prompt-injection-papers|New prompt injection papers]].)
- **Filtering/guardrails are not a defense** — "95% is a failing grade" in security; "using more AI to detect the attacks… does not work 100% reliably, which means it's not a useful security defense at all." Defenses keep falling to *adaptive* attacks (>90% success vs 12 published defenses). ([[2025-11-02-blog-willison-new-prompt-injection-papers|Attacker Moves Second]].)
- **The only credible end-user defense is a sandbox** — and **cutting network egress is the load-bearing control** because it severs the exfiltration leg of the trifecta. "The best sandboxes run on someone else's computer." ([[2025-10-22-blog-willison-living-dangerously-with-claude|Living dangerously with Claude]].)
- **"Agent" = an LLM that runs tools in a loop to achieve a goal** — a deliberately deflationary, useful definition he adopted in Sept 2025 after years of refusing the word. On that definition, agents are real and "extraordinarily useful," but narrow: **coding and search are the breakout categories**, not the sci-fi general assistant. ([[2025-12-31-blog-willison-the-year-in-llms|2025: the year in LLMs]].)
- **Coding agents crossed a capability threshold in Nov 2025** (GPT-5.1 + Claude Opus 4.5): from "mostly works, watch it closely" to "almost always does what you told it." Software engineers are the **bellwether** for all knowledge work — code came first because it's cheapest to verify. ([[2026-04-02-blog-willison-lennys-podcast|Lenny's Podcast]].)
- **The bottleneck has moved from the model to the human** — testing, verification, prototyping, and *agency*. "The one thing AI can never have is agency… invest in your own agency." (Converges with [[nathan-lambert|Lambert]]'s independent "agents push humans up the org chart" read.)
- **Pragmatic optimist on agent utility, hard skeptic on security hype** — and a persistent worry that "until there's a high-profile incident it's really hard to get people to take [prompt injection] seriously."
- **Coding agents** *are* **general agents** — Claude Code is "a general agent disguised as a developer tool"; Claude Cowork is that thesis shipped to non-developers. ([[2026-01-12-blog-willison-claude-cowork|Claude Cowork]].)

**Evolution 2025 → 2026:** Early 2025 he's a **tools-and-models explainer** — annotated release notes, local-model experiments (MLX, llama.cpp, sub-100MB LLMs), "vibe coding" coinage commentary, and a running skepticism that "agents" mean anything. Mid-2025 his **security** thread crystallizes into durable, lab-cited frameworks: the **design patterns** post (Jun 13), **lethal trifecta** (Jun 16), then the Lethal Trifecta talk circuit. Through autumn 2025 he flips from agent-skeptic to **agent power-user** — "YOLO mode," parallel coding agents, "vibe engineering" — while pairing every enthusiasm with a sandbox caveat (Living Dangerously, Oct). By the Dec year-in-review he's settled the definitional fight ("tools in a loop") and named the security tax as a permanent feature. In **2026** the lens widens to **general agents for everyone** (Claude Cowork, ChatGPT Containers, Datasette Agent) and to the **labor/skill implications** — the Nov-2025 inflection point, "dark factories," engineers-as-bellwether (Lenny's Podcast, Apr), and a candid note on how exhausting and addictive the new workflow is. Throughline across both years: the same disinterested security spine, applied to an ever-wider blast radius as agents go mainstream.

## Relationships
- writes at: simonwillison.net; creator of Datasette and the `llm` CLI; co-creator of Django (independent — see affiliation)
- coined "prompt injection" and "lethal trifecta" → [[agent-security]] · [[tool-description-poisoning]]
- weighs in on: [[agent-security]] · [[coding-agents]] · [[tool-use]] · [[agentic-ai]] · [[agent-protocols]] · [[mcp]] · [[agent-evaluation]] · [[agent-reliability]] · [[deep-research-agents]]
- recurring subjects: [[claude]] · [[anthropic]] · [[openai]] · [[mcp]]
- agent-definition crowdsourcing seeds [[swyx]]'s IMPACT taxonomy (he adds the security counterweight) → [[2025-03-24-blog-swyx-agent-engineering]]
- parallel "human-leverage" read to [[nathan-lambert]] (independent convergence on the bottleneck moving to the human)
- positions in [[debate-prompt-injection-solvable]] · ally of the "constrain the agent" side in [[debate-agents-vs-workflows]]

## Writings (agent-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage. (Pure link-blog and non-agent posts — release notes, image models, local-model fun — are omitted.)
- 2025-01-10 — My AI/LLM predictions for the next 1, 3 and 6 years (for Oxide and Friends) — https://simonwillison.net/2025/Jan/10/ai-predictions/
- 2025-03-02 — Hallucinations in code are the least dangerous form of LLM mistakes — https://simonwillison.net/2025/Mar/2/hallucinations-in-code/
- 2025-03-11 — Here's how I use LLMs to help me write code — https://simonwillison.net/2025/Mar/11/using-llms-for-code/
- 2025-03-19 — [[2025-03-19-blog-willison-not-all-vibe-coding|Not all AI-assisted programming is vibe coding (but vibe coding rocks)]]
- 2025-04-09 — Model Context Protocol has prompt injection security problems — https://simonwillison.net/2025/Apr/9/mcp-prompt-injection/
- 2025-04-11 — CaMeL offers a promising new direction for mitigating prompt injection attacks — https://simonwillison.net/2025/Apr/11/camel/
- 2025-04-21 — AI assisted search-based research actually works now — https://simonwillison.net/2025/Apr/21/ai-assisted-search/
- 2025-05-15 — Building software on top of Large Language Models — https://simonwillison.net/2025/May/15/building-on-llms/
- 2025-05-27 — Large Language Models can run tools in your terminal with LLM 0.26 — https://simonwillison.net/2025/May/27/llm-tools/
- 2025-05-31 — How often do LLMs snitch? Recreating Theo's SnitchBench with LLM — https://simonwillison.net/2025/May/31/snitchbench-with-llm/
- 2025-06-13 — Design Patterns for Securing LLM Agents against Prompt Injections — https://simonwillison.net/2025/Jun/13/prompt-injection-design-patterns/
- 2025-06-15 — An Introduction to Google's Approach to AI Agent Security — https://simonwillison.net/2025/Jun/15/ai-agent-security/
- 2025-06-16 — [[2025-06-16-blog-willison-lethal-trifecta|The lethal trifecta for AI agents]]
- 2025-08-09 — My Lethal Trifecta talk at the Bay Area AI Security Meetup — https://simonwillison.net/2025/Aug/9/bay-area-ai/
- 2025-08-15 — The Summer of Johann: prompt injections as far as the eye can see — https://simonwillison.net/2025/Aug/15/the-summer-of-johann/
- 2025-09-18 — I think "agent" may finally have a widely enough agreed upon definition to be useful jargon now — https://simonwillison.net/2025/Sep/18/agents/
- 2025-09-30 — Designing agentic loops — https://simonwillison.net/2025/Sep/30/designing-agentic-loops/
- 2025-10-05 — Embracing the parallel coding agent lifestyle — https://simonwillison.net/2025/Oct/5/parallel-coding-agents/
- 2025-10-07 — [[2025-10-07-blog-willison-vibe-engineering|Vibe engineering]]
- 2025-10-16 — Claude Skills are awesome, maybe a bigger deal than MCP — https://simonwillison.net/2025/Oct/16/claude-skills/
- 2025-10-20 — Claude Code for web — a new asynchronous coding agent from Anthropic — https://simonwillison.net/2025/Oct/20/claude-code-for-web/
- 2025-10-22 — [[2025-10-22-blog-willison-living-dangerously-with-claude|Living dangerously with Claude]]
- 2025-10-22 — Dane Stuckey (OpenAI CISO) on prompt injection risks for ChatGPT Atlas — https://simonwillison.net/2025/Oct/22/openai-ciso-on-atlas/
- 2025-11-02 — [[2025-11-02-blog-willison-new-prompt-injection-papers|New prompt injection papers: Agents Rule of Two and The Attacker Moves Second]]
- 2025-11-06 — Code research projects with async coding agents like Claude Code and Codex — https://simonwillison.net/2025/Nov/6/async-code-research/
- 2025-12-18 — Your job is to deliver code you have proven to work — https://simonwillison.net/2025/Dec/18/code-proven-to-work/
- 2025-12-31 — [[2025-12-31-blog-willison-the-year-in-llms|2025: The year in LLMs]]
- 2026-01-08 — LLM predictions for 2026, shared with Oxide and Friends — https://simonwillison.net/2026/Jan/8/llm-predictions-for-2026/
- 2026-01-12 — [[2026-01-12-blog-willison-claude-cowork|First impressions of Claude Cowork, Anthropic's general agent]]
- 2026-01-26 — ChatGPT Containers can now run bash, pip/npm install packages, and download files — https://simonwillison.net/2026/Jan/26/chatgpt-containers/
- 2026-02-07 — How StrongDM's AI team build serious software without even looking at the code — https://simonwillison.net/2026/Feb/7/software-factory/
- 2026-02-23 — Writing about Agentic Engineering Patterns — https://simonwillison.net/2026/Feb/23/agentic-engineering-patterns/
- 2026-03-14 — My fireside chat about agentic engineering at the Pragmatic Summit — https://simonwillison.net/2026/Mar/14/pragmatic-summit/
- 2026-04-02 — [[2026-04-02-blog-willison-lennys-podcast|Highlights from my conversation about agentic engineering on Lenny's Podcast]]
- 2026-04-03 — The Axios supply chain attack used individually targeted social engineering — https://simonwillison.net/2026/Apr/3/supply-chain-social-engineering/
- 2026-05-06 — Vibe coding and agentic engineering are getting closer than I'd like — https://simonwillison.net/2026/May/6/vibe-coding-and-agentic-engineering/
- 2026-05-21 — Datasette Agent — https://simonwillison.net/2026/May/21/datasette-agent/
- 2026-05-27 — I think Anthropic and OpenAI have found product-market fit — https://simonwillison.net/2026/May/27/product-market-fit/

## Cited by (posts)
- [[2025-03-19-blog-willison-not-all-vibe-coding]]
- [[2025-10-07-blog-willison-vibe-engineering]]
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-06-16-blog-willison-lethal-trifecta]]
- [[2025-10-22-blog-willison-living-dangerously-with-claude]]
- [[2025-11-02-blog-willison-new-prompt-injection-papers]]
- [[2025-12-31-blog-willison-the-year-in-llms]]
- [[2026-01-12-blog-willison-claude-cowork]]
- [[2026-04-02-blog-willison-lennys-podcast]]
