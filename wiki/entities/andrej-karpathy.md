---
type: entity
entity_type: person
aliases: [karpathy]
tags: [agents, person]
affiliation: "Joined Anthropic's pre-training team May 19 2026 (using Claude to accelerate pre-training research, under Nick Joseph); founder of Eureka Labs (AI education, 2024) — framed as deferred, not closed; ex-OpenAI (founding member) and ex-Tesla (Sr. Director of AI / Autopilot). Writes at karpathy.bearblog.dev."
stake: Educator / communicator — coiner of the field's vocabulary (vibe coding, Software 1.0/2.0/3.0, jagged intelligence, ghosts-vs-animals). Low product/fund book; reads as genuine framing. NOTE the new Anthropic affiliation (May 2026) — discount future model/pre-training takes accordingly.
url: https://karpathy.bearblog.dev/
created: 2026-06-22
updated: 2026-06-22
---

# Andrej Karpathy

*The field's foremost teacher-communicator — coined [[vibe-coding|vibe coding]], "Software 3.0," "jagged intelligence" and "ghosts vs animals," and articulates the agentic shift more legibly than anyone. As of May 2026 he's at [[anthropic|Anthropic]] on pre-training; the radar's most quotable perspective voice on what LLMs **are** and how to build with them.*

## Who they are
A founding member of [[openai|OpenAI]] and former Sr. Director of AI at Tesla (led Autopilot's vision stack), who left to found **Eureka Labs** (AI-native education, 2024). On **May 19 2026** he joined **[[anthropic|Anthropic]]'s pre-training team** to use Claude to accelerate pre-training research (under Nick Joseph) — explicitly framing Eureka Labs as deferred, not closed. He writes durable conceptual essays at **karpathy.bearblog.dev** (started March 2025) and ships educational artifacts (nanochat, microGPT, LLM101n). His lens is **educator/communicator first** — he names the abstractions the rest of the field then argues with.

**Stake:** Low commercial book historically — no model or fund to sell, which is why his framings travel so far. That changes somewhat with the **Anthropic move (May 2026)**: weight his future pre-training / model-capability takes at a modest discount, and note that pieces like the Sequoia Ascent write-up are pitched partly to founders at a VC venue. His RL/architecture reads carry weight (it's his domain); his predictions are framings, not forecasts.

## What they argue (recurring stances)
- **LLMs are a new computing paradigm — "Software 3.0."** Software 1.0 = hand-written code; 2.0 = learned weights; **3.0 = programming the LLM through the context window** (prompts, tools, memory, instructions). The context window is the new program; some apps "should stop existing as apps" because the model does the transformation directly. ([[2026-04-30-blog-karpathy-sequoia-ascent-2026|Sequoia Ascent 2026]], building on his Software 2.0 thesis.)
- **Verifiability governs the jagged frontier.** "Traditional software automates what you can *specify*; LLMs/RL automate what you can *verify*." Capability spikes where tasks are verifiable AND labs spent training attention (`verifiability × training attention × data coverage × economic value`) — hence models can refactor a 100k-line codebase yet tell you to *walk* to a car wash 50m away. (His *Verifiability* post, Nov 2025; relates to [[agent-evaluation]].)
- **Ghosts, not animals.** Frontier LLM research isn't "growing animals," it's "summoning ghosts" — statistical distillations of human text, jagged and alien, not intrinsically-motivated minds. Anthropomorphic intuitions mislead; the right posture is empirical familiarity. (His *Animals vs Ghosts* post, Oct 2025, responding to Sutton on Dwarkesh.)
- **Vibe coding raises the floor; agentic engineering raises the ceiling.** He **coined [[vibe-coding|vibe coding]]** (Feb 6 2025) — building by prompting and accepting unread diffs — then by 2026 drew the line to **agentic engineering**: the professional discipline of coordinating fallible agents while preserving correctness, security, taste (specs, diff review, tests, evals, permissions, isolated worktrees). Vibe coding for prototypes; agentic engineering for serious software.
- **LLMs diffuse bottom-up — "power to the people."** Uniquely among transformative technologies, LLMs benefit individuals first and corporations/governments later (org complexity, control needs, and inertia slow adoption). Contingent on frontier performance staying cheap/flat — if the dynamic range widens, advantage re-concentrates toward whoever can spend. ([[2025-04-07-blog-karpathy-power-to-the-people|Power to the people]].)
- **"You can outsource your thinking, but not your understanding."** Even as agents do the work, human understanding stays the bottleneck for directing them — which is why he champions **LLM knowledge bases** (the [[llm-wiki]] pattern) as understanding tools, not just answer machines.

**Evolution 2025 → 2026:** Early 2025 he's framing *diffusion and empowerment* (Power to the People; coining vibe coding). Mid/late 2025 he turns to *what LLMs are* — Verifiability, Animals vs Ghosts, The Space of Minds — building the conceptual vocabulary for jaggedness. By the **December 2025 agentic inflection** ("never felt more behind as a programmer") he pivots to *how to build* — Software 3.0, agentic engineering, agent-native infrastructure — landing in the Sequoia Ascent synthesis just before joining Anthropic.

## Relationships
- writes at: karpathy.bearblog.dev; ships nanochat / microGPT / LLM101n (education)
- affiliated with [[anthropic]] (pre-training, May 2026); founder of Eureka Labs; ex-[[openai]]
- **coined** [[vibe-coding]]; weighs in on [[coding-agents]] · [[agent-adoption]] · [[agent-evaluation]] · [[llm-wiki]] · [[agentic-ai]] · [[distillation]]
- recurring subjects: [[claude]] · [[mcp]] · [[reasoning-models]]
- perspective counterpart on practitioner workflow: [[nathan-lambert]] · [[simon-willison]] (sharpened his vibe-coding definition)

## Writings (agent-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage. All at karpathy.bearblog.dev unless noted.
- 2025-03-17 — Digital hygiene — https://karpathy.bearblog.dev/digital-hygiene/
- 2025-03-19 — The append-and-review note — https://karpathy.bearblog.dev/the-append-and-review-note/
- 2025-03-24 — Finding the Best Sleep Tracker — https://karpathy.bearblog.dev/finding-the-best-sleep-tracker/
- 2025-04-07 — [[2025-04-07-blog-karpathy-power-to-the-people|Power to the people: How LLMs flip the script on technology diffusion]]
- 2025-04-27 — Vibe coding MenuGen — https://karpathy.bearblog.dev/vibe-coding-menugen/
- 2025-10-01 — Animals vs Ghosts — https://karpathy.bearblog.dev/animals-vs-ghosts/
- 2025-11-17 — Verifiability — https://karpathy.bearblog.dev/verifiability/
- 2025-11-29 — The space of minds — https://karpathy.bearblog.dev/the-space-of-minds/
- 2025-12-10 — Auto-grading decade-old Hacker News discussions with hindsight — https://karpathy.bearblog.dev/auto-grade-hn/
- 2025-12-18 — Chemical hygiene — https://karpathy.bearblog.dev/chemical-hygiene/
- 2025-12-19 — 2025 LLM Year in Review — https://karpathy.bearblog.dev/year-in-review-2025/
- 2026-04-30 — [[2026-04-30-blog-karpathy-sequoia-ascent-2026|Sequoia Ascent 2026 summary (Software 3.0 / Agentic Engineering / Jagged Intelligence)]]

*Note: several marquee Karpathy pieces are talks/podcasts (Dwarkesh pod, Y Combinator talk, the Sequoia Ascent fireside itself) — see TRANSCRIPT BACKLOG. The Sequoia Ascent write-up was captured because he published a fetchable written summary + transcript.*

## Cited by (posts)
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-04-07-blog-karpathy-power-to-the-people]]
- [[2026-04-30-blog-karpathy-sequoia-ascent-2026]]
