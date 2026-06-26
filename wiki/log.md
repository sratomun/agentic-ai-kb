## [2026-06-22] deep-ingest | full-text ingested 36 canonical papers behind the frontier-model-production cluster
- Ran 6 parallel ingest agents (2 interrupted + resumed): each fetched full text via alphaXiv, saved raw/arxiv/{id}.fulltext.md, wrote a grounded deep source note (real numbers from paper body, no fabrication).
- Stages: data corpora (Pile, T5/C4, RefinedWeb, FineWeb, DCLM, DoReMi, Dedup); synthetic+tokenization (Self-Instruct, phi-1, Distilling Step-by-Step, WebSailor-V2, BPE, SentencePiece); pretraining+scaling (GPT-3, Kaplan, Chinchilla, Emergent Abilities, Emergence-Mirage, Compute Trends, DeepSeek-V3); MoE (Sparse-MoE, GShard, Switch, Mixtral, DeepSeekMoE); post-training (InstructGPT, Tülu 3, Llama 2/3, DeepSeek-R1, LIMA, RM-Overoptimization, DPO, Constitutional AI, RLAIF); distillation (Hinton, Seq-KD, DistilBERT).
- Upgraded all 12 supply-side nodes: replaced the "queued for deep ingest" manifests with wikilinked "## Key papers (full-text ingested)" sections carrying verified figures; concept evidence now grounded in real source notes.
- Updated index.md Sources (new deep-ingest group). Integrity: fixed 7 display-text-as-slug links in agent notes ([[Scaling laws]]→[[scaling-laws|...]], [[meta]]→[[meta-ai]], [[gpt-3]]→plain); 0 broken links across the 36 notes + 12 nodes.
- Open: citationCount omitted on most notes (alphaXiv didn't surface counts); kg-curator can backfill from Semantic Scholar. One degraded capture: Constitutional AI (2212.08073) full-text timed out → depth: report, qualitative only.

## [2026-06-22] extend | new supply-side cluster "frontier model production" (references-first scaffold, option b)
- New hub [[frontier-model-training]] as the supply-side mirror of [[agentic-ai]]; wired inbound from agentic-ai, reasoning-models, open-models.
- New stage concepts: [[pretraining]], [[pretraining-data]] (absorbs curation/dedup), [[synthetic-data]], [[scaling-laws]], [[mixture-of-experts]], [[post-training]] (hub), [[distillation]].
- New method/person entities: [[sft]], [[reward-modeling]], [[constitutional-ai]], [[tokenization]], [[lilian-weng]].
- Folded (no standalone node, per references bar): quantization → [[open-models]] efficiency note; training-compute → [[nvidia]]/[[vera-rubin]] + cross-ref [[scaling-laws]].
- Every node references-backed: wikilinks to existing local blog notes for grounding + a verified canonical-arXiv manifest ("queued for deep ingest") on each. ~30 canonical arXiv IDs vetted by 4 parallel research subagents (local-first, then arXiv verification). No invented findings/numbers per STYLE grounding rule.
- Reciprocal backlinks added to agentic-ai, reasoning-models, open-models, agent-security, rlhf, dpo, ppo, grpo, rlvr, deepseek, anthropic, nvidia, vera-rubin. Updated index.md (new "Frontier model production" group). Integrity: 0 broken links across new+edited files; all 13 new nodes non-orphan.
- Follow-up for arxiv-scanner/kg-curator: deep-ingest the canonical manifests into source notes; create blog source note for Lilian Weng reward-hacking (raw/blogs/2024-11-28).

## [2026-06-22] ingest | promoted 7 functional-task eval papers from census to browsable KG (Cloud-OpsBench, Insight-Agents, JAF, BIRD-Python, Text-to-Big-SQL, LLM4Cov, DECKBench); added concepts llm-as-judge + data-analysis-agents; updated agent-evaluation, data-query-agents, agent-reliability
## [2026-06-22] ingest | full-text ingested the 7 functional-task eval papers (Cloud-OpsBench, Insight-Agents, JAF, BIRD-Python, Text-to-Big-SQL, LLM4Cov, DECKBench); upgraded notes abstract->full-text with verified metrics/figures; refreshed report + entities + concepts

## 2026-06-22 — Perspective-layer holistic sweep (2025–26)
- Ran blog-scanner with scope=2025&2026 as a run parameter (not baked into the skill). No pre-2025 captures deleted — older posts remain as genealogy/debate anchors.
- Holistic per-author subagents: upgraded [[simon-willison]] (thin→holistic, 6 deep notes); new [[sebastian-raschka]], [[chip-huyen]], [[hamel-husain]], [[ethan-mollick]].
- Lab blogs: new [[google-deepmind]], [[hugging-face]], [[mistral-agents-api]] (org [[mistral]] pre-existed); 6 deep lab source notes.
- New hubs: [[agent-adoption]] (concept), [[open-models]] (concept), [[inspect-ai]] (framework), [[debate-evals-vs-frameworks]] (debate).
- Wired reciprocal backlinks into agent-evaluation, coding-agents, reasoning-models, agentic-ai, agent-security, multi-agent-systems, mcp, google, mistral, debate-agents-vs-workflows.
- Incidental product/person mentions (Braintrust/LangSmith/Phoenix/Parlance Labs/Shreya Shankar/Eugene Yan/GitHub) kept as plain text, not stub nodes.
- Lint: 0 broken links in wiki content; 0 orphans (excl. reserved log.md).

## 2026-06-22 — Developed vibe-coding & harness-engineering hubs
- New concepts: [[vibe-coding]] and [[harness-engineering]] (aliases agentic-engineering/vibe-engineering), grounded across both layers (arxiv: vibe-vs-agentic-coding, code-as-agent-harness; perspective: Willison, Raschka, swyx, Mollick, Husain, Lambert).
- Captured 2 canonical Willison posts: [[2025-03-19-blog-willison-not-all-vibe-coding]] (definition + Karpathy origin) and [[2025-10-07-blog-willison-vibe-engineering]].
- Wired into coding-agents, agentic-ai, agent-evaluation, debate-evals-vs-frameworks; re-linked Husain's "harness engineering" mention; index updated.

## 2026-06-22 — Frontier-lab blogs + lab-researcher voices
- OpenAI blog sweep: 6 deep notes (Deep Research, Agents SDK/Responses, Codex, ChatGPT agent, AgentKit, practical guide).
- Anthropic blog sweep: 5 deep notes (multi-agent research system, writing tools for agents, context engineering, code execution with MCP, long-running harnesses). MCP origin now stated on [[anthropic]].
- Lab researchers (written long-form): new [[jason-wei]] (Meta SI Labs, ex-OpenAI) + [[jan-leike]] (Anthropic alignment, ex-OpenAI); 5 deep notes.
- Wired backlinks into openai/anthropic/meta-ai/mcp + agentic-ai, tool-use, computer-use-agents, deep-research-agents, coding-agents, reasoning-models, agent-evaluation, agent-security, multi-agent-systems, harness-engineering, chain-of-thought, debate-llms-path-to-agi.
- Shortlist for next pass (written-first, then transcripts): Karpathy (now Anthropic, May 2026), Jack Clark/Import AI essays, Neel Nanda, Chris Olah, Lilian Weng ("Why We Think"). Then priority-3 commentary: Hinton, Hassabis, Jeff Dean.

## 2026-06-22 — Commentary figures + lab-researcher shortlist (written-first)
- New person nodes: [[demis-hassabis]], [[geoffrey-hinton]], [[jeff-dean]], [[andrej-karpathy]], [[jack-clark]], [[neel-nanda]], [[lilian-weng]]. ~16 deep source notes (essays + published transcripts; NO Chrome this run).
- New nodes: [[thinking-machines-lab]] (org), [[debate-ai-existential-risk]] (Hinton/Leike/Clark vs LeCun/Lambert).
- Wired voices into agentic-ai, reasoning-models, world-models, science-agents, frontier-model-governance, governance-gap, agent-security, self-evolving-agents, llm-wiki, agent-adoption, vibe-coding (Karpathy as originator), chain-of-thought + org nodes; debate-llms-path-to-agi gained Hassabis/Hinton/Wei/Leike.
- TRANSCRIPT BACKLOG (needs serial Chrome pass): Hassabis (WIRED/Levy, India AI Summit, Rundown AGI, I/O 2026, GDM podcast); Hinton (Ai4 2025 "AI mothers" keynote, CNN Dec-2025); Jeff Dean (Sequoia AI Ascent, GDM podcast, NVIDIA GTC); Karpathy (Dwarkesh 2025, YC Software 3.0); Hinton CBS Mornings is fetchable-next.

## 2026-06-23 — Small Language Models: new hub + entities + census backfill
- New concept hub [[small-language-models]] (kind: domain), full-text-grounded on Belcak et al. (NVIDIA, 277 cites — top-cited paper in the census): SLM-first agentic economics (7B ≈ 10–30× cheaper than 70–175B), capability evidence (Phi/Nemotron/SmolLM/DeepSeek-R1-Distill/xLAM), the LLM→SLM conversion algorithm, and the non-technical adoption barriers. Caveats wired (structured-output reliability, reasoning-depth limits) + vendor-stake discount.
- New model entities: [[phi]] (Microsoft), [[nemotron]] (NVIDIA, incl. Hymba), [[smollm]] (HuggingFace), [[gemma]] (Google, 98 census mentions).
- Backfilled 84 browsable abstract notes (depth: abstract) for census SLM papers across 2025/2026, keyword-linked to the hub + tool-use/memory/judge/on-device concepts.
- Reciprocal links added on agentic-ai, distillation, open-models, mixture-of-experts, reasoning-models, post-training, tool-use, agent-memory, agent-reliability, multi-agent-systems, intent-routing, intent-understanding, qwen, deepseek; SLM hub added to the Belcak deep note's concept links.
- Dropped 4 false-positive census matches (1-bit bandit/safety papers, million-agent scaling) and a duplicate Belcak note.

## 2026-06-23 — SLM sub-concepts split out (on-device, judge, memory)
- Promoted the 3 folded SLM sub-themes from [[small-language-models]] into first-class nodes: [[on-device-agents]] (~30 papers; full-text-grounded on Belcak — ChatRTX/PowerInfer/Dynamo edge economics; recent: Ferret-UI Lite, MobileExplorer, KVNAND, MobileFineTuner, BitRL, QKVShare, Agent-X; caveat GhostEI-Bench), [[slm-as-judge]] (~8; SLMJury/JudgeBoard; reasoning-depth caveat), [[slm-agent-memory]] (~9; MemFlow/CLAG/ScrapMem).
- Hub "Includes" replaced with a "Sub-concepts (split out)" section + relationship links.
- Reciprocal links added on llm-as-judge, agent-memory, computer-use-agents, agent-security, agentic-rag, post-training, recommendation-agents. Index updated (3 new concept lines).
## 2026-06-23 lint | +on-device-agents/slm-as-judge/slm-agent-memory + enrich (citation-ranked Key papers/Cited by on hub, 3 sub-concepts, 4 entities). 0 broken, 0 orphans.
## 2026-06-23 lint+enrich | graph-wide enrich pass: citation-ranked Key papers/Cited by on 6 nodes with real census data (llm-as-judge, mediated-semantic-architecture, data-analysis-agents, intent-understanding, intent-routing, text-to-cypher); curated lists restored on intent-grounding/semantic-parsing/text-to-sql (no fabricated counts); merged duplicate Cited-by on gaia/swe-bench/osworld/bfcl; reverted speculative all-zero sections; preserved curated full-text lists. 0 broken, 0 orphans, 0 dup sections.

## [2026-06-23] ingest | Security standards layer — NIST, OWASP, MITRE ATLAS, CSA MAESTRO
Completed the agentic-security graph with its missing reference scaffolding. New concept hub [[security-standards]] organizes the four complementary frameworks along the autonomy spectrum (raw LLM call → single-turn tool agent → autonomous/multi-agent). Added 4 org nodes ([[nist]], [[owasp]], [[mitre]], [[cloud-security-alliance]]) + 5 framework nodes ([[nist-ai-rmf]], [[owasp-llm-top-10]], [[owasp-agentic-top-10]], [[mitre-atlas]], [[maestro]]), all reciprocally linked. Wired the autonomy-spectrum axis into [[agent-security]] and backlinks into [[governance-gap]]. Generated cyber-team report `agentic-security-playbook-2026.md`.
