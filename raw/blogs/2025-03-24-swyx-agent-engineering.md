# Agent Engineering

- Author: swyx (Shawn Wang)
- Outlet: Latent.Space
- URL: https://www.latent.space/p/agent
- Date: 2025-03-24
- Fetched: 2026-06-22
- Note: elaborations on swyx's 2025 AI Engineer Summit keynote.

---

"After some debate, we finally decided to take 'agent engineering' head on." First task:
defining agents.

## Defining Agents: A Linguistic Approach
Simon Willison loves asking people their agent definitions — "it is an open secret that
nobody agrees, and therefore debates about agent problems and frameworks are
near-impossible since you can set the bar as low or as high as you want." "People always
overemphasize where they start from and trivialize every perspective that doesn't."

Even within OpenAI definitions disagree. OpenAI's Agents SDK working definition (swyx
acronymizes "TRIM"): an AI application = a model + instructions + tools, encapsulated in
a runtime with a dynamic lifecycle. But TRIM forgets planning and memory, vs Lilian
Weng's "Agent = LLM + memory + planning skills + tool use."

"Achieving common understanding of a word is... a linguistic [matter]. The most robust
approach is descriptive, not prescriptive." Simon collected 250+ replies; swyx did the
last-mile reading/grouping.

## The Six Elements of Agent Engineering (IMPACT backronym)
Ranked in rough descending order of commonality/importance:
- LLMs with **Tools**: the thing everyone agrees on. Big 3 "LLM OS" tools are RAG/Search,
  Sandboxes/Canvas, Browsers/CUA. (Weng)
- Encoded **Intent**: intents come in via multimodal I/O, encoded in Goals and verified
  via Evals run in Environments. ("goal-oriented behavior, adapt along the way" — Rutherford)
- LLM-Driven **Control Flow**: LLMs-in-the-loop is the common line between preset
  "Workflows" and autonomous "Agents." ("The more agentic an application is, the more an
  LLM decides the control flow" — Harrison Chase)
- Multi Step **Planning**: SOTA is editable plans (Deep Research, Devin/Manus). ("non-trivial,
  multi-step operations that previously would have required a human" — Daniel Miessler)
- Long Running **Memory**: creates coherence and self-improvement loops. Beyond
  MemGPT/MCP memory, also Voyager/SteP-style reusable workflows and skill libraries as a
  more structured form of memory. ("long running, open ended tasks in the real world" — Jeffries)
- Delegated **Authority**: "Trust is the most overlooked element and yet the oldest"
  (principal-agent problem). "Stutter-step agents" (asking confirmation before every
  action) get old fast; Trust but Verify for read-heavy workflows, enterprise needs more.
  ("An agent is trusted to act on behalf of... If there's no trust there is no agent." — Pshichenko)

"You can FEEL when an agent forgets one of these 6 things. OpenAI's TRIM agent framework
has no emphasis on memory, planning, or auth."

## Agents, Hot and Cold
Chronicles the sentiment cycle: Spring 2023 AutoGPT/BabyAGI excitement → Fall 2023-Spring
2024 nadir ("Why AI Agents Don't Work (yet)", custom GPTs flop, "Winds of AI Winter",
"agents had become a bad word in Silicon Valley") → Summer 2024 rebound (CrewAI, Agentic
RAG) → Fall 2024 reasoning models (o1, Claude 3.5 Sonnet doubling Anthropic's share) →
Winter-Spring 2025 OpenAI Operator + Deep Research, "All In on Agent Engineering" for NYC.

ChatGPT's growth tracks reasoning/agent model releases. METR: the agent task horizon
doubles every 3-7 months.

## Why work on Agent Engineering Now?
Obvious catalysts: better models (reasoning, coding), better tool use (100% structured
output, BFCLv3/IFEval), better tools (Big 3 + MCP winning the long tail).
Slow-burn trends: business model shifts ($2-20k ChatGPT, Sierra charging for outcomes),
1000x Moore's Law (reasoning cost drop), >100x inference (speculative editing, ASICs →
5000 tok/s), model diversity, multi-agent research, RL finetuning.

Footnote 3: Ramp's talk frames workflow-vs-agent as a Bitter Lesson — "workflows get you
far in the short term, but often get steamrolled by the next order of magnitude gain in
intelligence or cost/intelligence."

"This is why there's a new resurgence in agents and the field of Agent Engineering is
just now becoming the hottest thing in AI Engineering."
