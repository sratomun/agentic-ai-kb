# The Agent Labs Thesis (Welcome to GPT Wrapper Summer)

- Author: swyx (Shawn Wang)
- Outlet: Latent.Space
- URL: https://www.latent.space/p/agent-labs
- Date: 2025-11-18
- Fetched: 2026-06-22

---

swyx disagrees with Steph Palazzolo's "Neolab" coinage; for AI Engineer Code Summit he
used "**Agent Lab**" instead. Neolabs = "Neolabs that exploit new approaches to developing
AI models and research that OpenAI and Anthropic have overlooked" (Thinking Machines, SSI,
Reflection). Agent Labs cover an orthogonal trend: Cursor ($29B), Perplexity ($20B),
Cognition ($10B), Sierra ($10B), Lovable ($2B), Gamma ($2B), plus AI-transitioned
companies (Notion $10B, Vercel $9B, Glean $7B, Replit $3B), and "Agent Labs within Model
Labs" (Claude Code $1B ARR, Codex, Google Labs).

"Just being 'new' isn't a business plan." "Agent Labs have their business plan embedded in
the name: where Model Labs primarily research and sell models, Agent Labs primarily
research and sell agents."

## Differences between Model Labs vs Agent Labs
- **Product First, Model Last**: Cursor forked VSCode first, understood user needs for 2
  years, THEN worked on the model. (vs Magic.dev raising $100m for a long-context model.)
- **Outcome-based Pricing or Marketing**: Model Labs are on a 9-900x/year distillation
  grind with little pricing power (exception: Anthropic); maxed-out $20/mo subs. Agent Labs
  can charge $2000/month or per outcome — higher margins, pricing power, growth, "because
  you measurably replace some subsection of human labor."
- **Approach to autonomy**: Model Labs take control away from the user (prioritize hours of
  autonomy, lightweight harnesses like Building Effective Agents and Skills, believing the
  next model upgrade might undo harness gains). Agent Labs prioritize speed,
  auditable/human-in-the-loop control and multiturn interactivity, and "don't mind
  rewriting the harness every few months."
- **Evals/metrics**: Model Lab charts are often 1-dimensional (max capability ignoring
  cost, e.g. IMO, IOI). Agent Labs care about the pareto frontier of intelligence/success
  vs cost.

Conway's Law is the biggest tell: a company's priorities show in resource allocation.
Model labs pay "Applied AI Engineers" ~half what they pay research staff. Another tell:
how willingly they "drop alpha" / open source agents (OpenAI shared sales/support/research
agents; Vercel shared 5 agents) — "commoditize your complements."

## It is Open Season for Agent Labs
Two datapoints: (1) Epoch estimates ALL of OpenAI inference (ChatGPT, Sora, Codex, API,
internal) is only ~28% of their compute — the majority goes to unpublished fundamental
research, "as it should be." (2) The OpenAI Foundation livestream where Sam said "AI Cloud",
"Third Party apps," and quoted the Bill Gates Line for the first time — "Sam has never, ever,
spoken so clearly about OpenAI's intention to serve third party builders at the app layer."
"OpenAI achieves the most scale by going DOWN the stack... far more likely to achieve AGI
that way than by going UP the stack." Anthropic ($350B raise, first $50B datacenter) is the
most serious contender.

"One year on from writing Why GPT Wrappers are Good, Actually, we now actually have official
blessing from leading frontier labs that they are finally taking AI Engineers more seriously."

## Why Agent Labs Now?
- **Priorities**: Model Labs prioritize AGI models (<30% budget on inference; products get
  abandoned — Operator, NotebookLM Audio, Scheduled Tasks, Deep Research); both OpenAI and
  Anthropic now signal building platforms for developers rather than first-party apps.
- **Model Diversity**: number of relevant frontier Model Labs has gone UP. "People want to
  pay someone to capabilitymaxx for them" — the full-time job of keeping up with SOTA and
  building the best model+harness for the task. "Agents are Systems. The Model Selector is a
  Lie" — agents are bundles of (model, prompt, memories, tools, planning, orchestration,
  auth), so model labs' end-to-end advantage declines.
- **Pretraining → RL**: ~7-13 years of pretraining scaling; near limits of pretraining data.
  "The RL age rewards domain focus/dedicated environments and matching/surpassing best
  humans." Grok 4 (3T params) shows roughly equal post-training and pretraining spend. Agent
  Labs (Cursor, Cognition) can start from powerful open weights and do continued training —
  Cursor's post-training may "largely make up the gap between the best open models and the
  best frontier models."

## The end of one size fits all?
Bear case: Agent Labs embedded in Model Labs grow so important they create a lasting fork in
the model tree. GPT5 has evaded omnimodality; GPT5 router issues, gpt-5-codex vs gpt-5
persistence, and Fidji Simo's "Moving beyond one-size-fits all" suggest the Model Lab "G"-in-
AGI vision might be shifting, at least until the next algorithm shift.
