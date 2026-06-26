# The 2025 AI Engineering Reading List

- Author: swyx (Shawn Wang) + Latent.Space team
- Outlet: Latent.Space
- URL: https://www.latent.space/p/2025-papers
- Date: 2024-12-27 (modified 2025-12-29; "continuously maintained")
- Fetched: 2026-06-22
- Note: mostly paywalled; the Agents section (section 5) and the framing captured here.

---

"We picked 50 paper/models/blogs across 10 fields in AI Eng: LLMs, Benchmarks, Prompting,
RAG, Agents, CodeGen, Vision, Voice, Diffusion, Finetuning. If you're starting from scratch,
start here." Updated from the 2023 a16z Canon with a practical focus.

Design goals: pick ~50 papers (one a week); tell you WHY each paper matters; be VERY
practical for the AI Engineer ("no time wasted on Attention is All You Need").

## Section 5: Agents (the agent-relevant core)
1. **SWE-Bench** & SWE-Lancer — "probably the highest profile agent benchmark today"
   (vs WebArena, SWE-Gym). "Technically a coding benchmark, but more a test of agents than
   raw LLMs." See also SWE-Agent, SWE-Bench Multimodal, Konwinski Prize. For
   Tool-Agent-User interaction: TauBench (Airlines/Retail) and GAIA.
2. **ReAct paper** — "ReAct started a long line of research on tool using and function
   calling LLMs," including Gorilla and the BFCL Leaderboard. Of historical interest:
   Toolformer, HuggingGPT.
3. **MemGPT paper** — "one of many notable approaches to emulating long running agent
   memory," adopted by ChatGPT and LangGraph. Reinvented in MetaGPT, AutoGen, Smallville.
4. **Voyager paper** — Nvidia's take on 3 cognitive-architecture components (curriculum,
   skill library, sandbox). Skill library/curriculum can be abstracted as Agent Workflow
   Memory.
5. **Anthropic on Building Effective Agents** — "just a great state-of-2024 recap that
   focuses on the importance of chaining, routing, parallelization, orchestration,
   evaluation, and optimization." See also Lilian Weng's Agents, Shunyu Yao on LLM Agents,
   Chip Huyen's Agents.

"We skipped bikeshedding agent definitions, but if you really need one, you could use mine."

## Other framing of note
- Reasoning models dominate the 2025 frontier (o1, o3, R1, QwQ/QVQ, f1); Sebastian Raschka's
  literature review recommended.
- Benchmarks saturate increasingly quickly; "there is a sense that the whole approach is
  getting dated and new approaches are needed."
- China models (Kimi K-2, Qwen 3) have overtaken in open models.
- Much of the agent/codegen frontier "has moved from research to industry" — only found in
  industry blogposts and talks rather than research papers.
