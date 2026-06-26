---
title: "Automating AI Research (Import AI 455, Import A-Idea essay)"
author: Jack Clark
outlet: Import AI (jack-clark.net / importai.substack.com)
url: https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/
date: 2026-05-04
captured: 2026-06-22
source_type: blog
note: "Import A-Idea essay section of Import AI #455 ('AI systems are about to start building themselves'). This whole issue is the essay (no separate paper-roundup digest). Captured near-verbatim with light elision of repeated transitions."
---

# Automating AI Research — AI systems are about to start building themselves. What does that mean?

*Import A-Idea essay, Import AI #455. Immutable.*

I'm writing this post because when I look at all the publicly available information I reluctantly come to the view that there's a likely chance (60%+) that no-human-involved AI R&D — an AI system powerful enough that it could plausibly autonomously build its own successor — happens by the end of 2028. This is a big deal. I don't know how to wrap my head around it... I now believe we are living in the time that AI research will be end-to-end automated. If that happens, we will cross a Rubicon into a nearly-impossible-to-forecast future.

In terms of timing, I don't expect this to happen in 2026. But I think we could see an example of a "model end-to-end trains its successor" within a year or two — certainly a proof-of-concept at the non-frontier model stage... My reasoning for this stems primarily from public information: papers on arXiv, bioRxiv, and NBER, as well as observing the products being deployed into the world by the frontier companies.

**The coding singularity — capabilities over time:** AI systems are instantiated via software and software is made out of code. AI systems have revolutionized the production of code.
- **SWE-Bench:** When it launched in late 2023 the best score was Claude 2 at ~2%. Claude Mythos Preview gets 93.9%, effectively saturating the benchmark. The vast majority of people I meet at frontier labs now code entirely through AI systems.
- **METR time horizons:** In 2022, GPT-3.5 could do tasks taking ~30 seconds. 2023: 4 minutes (GPT-4). 2024: 40 minutes (o1). 2025: ~6 hours (GPT 5.2 High). 2026: ~12 hours (Opus 4.6). Ajeya Cotra (METR) thinks ~100 hours by end of 2026 is not unreasonable.

**AI is getting good at core science skills essential to AI R&D:**
- **CORE-Bench** (reproduce a paper from its repo): Sept 2024 best was ~21.5% (GPT-4o in CORE-Agent); Dec 2025 an author declared it 'solved' with Opus 4.5 at 95.5%.
- **MLE-Bench** (Kaggle competitions): Oct 2024 top was 16.9% (o1 in scaffold); Feb 2026 best is 64.4% (Gemini3 + search harness).
- **Kernel design:** going from curiosity to competitive research area (DeepSeek GPU kernels, PyTorch→CUDA automation, Meta Triton kernels, Huawei Ascend "AscendCraft", "Cuda Agent" fine-tuning). Caveat: kernel design has easily verifiable rewards.
- **PostTrainBench** (fine-tune small open models): as of March 2026, AI systems get ~half the uplift of human researchers. Top systems (Opus 4.6, GPT 5.4) get 25-28% vs human baseline of 51%.
- **Optimizing LM training (Anthropic's CPU-only speedup task):** Opus 4 achieved 2.9× mean speedup (May 2025) → 16.5× Opus 4.5 (Nov 2025) → 30× Opus 4.6 (Feb 2026) → 52× Claude Mythos Preview (April 2026). A human researcher takes 4-8 hours to reach 4×.
- **Automated alignment research (Anthropic PoC, #454):** AI agents primed with a research direction beat a human-designed baseline on scalable oversight, at small scale, not yet generalizing to production.

**Meta-skills: management** — AI systems are learning to manage other AI systems (Claude Code / OpenCode, a single agent supervising sub-agents).

**Is AI research more like discovering general relativity or Lego?** My sense is that AI cannot yet invent radical new ideas — but the technology may not need to for it to automate its own development. As a field, AI moves forward mostly through "meat and potatoes" engineering: take a well-performing system, scale up some aspect, see what breaks, fix it, scale again. Edison: "genius is 1% inspiration and 99% perspiration." AI has got extremely good at the schlep components. Preliminary signs of creativity exist (Erdos problems: a Gemini model solved Erdős-1051 as an "early example of an AI autonomously resolving a slightly non-trivial open Erdős problem"; a centaur math proof built with Google Gemini), but these may be domains (CS, math) oddly amenable to AI invention. Move 37 hasn't been replaced in ten years — a weakly bearish signal.

**Putting it all together:** AI can write code for pretty much any program and be trusted on tasks taking a human tens of hours; AI is increasingly good at AI-development tasks (fine-tuning to kernel design); AI can manage other AI forming synthetic teams; AI can sometimes out-compete humans on hard engineering/science tasks. To me, this makes a very convincing case that AI can today automate vast swathes, perhaps the entirety, of *AI engineering*. It is not yet clear how much of AI *research* it can automate.

**The industry literally says AI R&D is its goal:** OpenAI wants an "automated AI research intern by September of 2026"; Anthropic publishes on automated alignment researchers; DeepMind says "automation of alignment research should be done when feasible." Recursive Superintelligence raised $500m to automate AI research; Mirendil aims to build "systems that excel at AI R&D."

**Why this matters:**
1. **We have to get alignment right.** Alignment techniques that work today may break under recursive self-improvement. Compounding-error problem: a 99.9%-accurate technique becomes 95.12% accurate after 50 generations, 60.5% after 500. Uh oh!
2. **Everything AI touches gets a massive productivity multiplier** — raising inequality-of-access (compute allocation becomes politically charged; market incentives don't guarantee best social upside) and an "Amdahl's Law for the economy" (weak links break, especially fast-digital vs slow-physical, e.g. drug trials).
3. **The formation of a capital-heavy, human-light economy** — a "machine economy" growing within the "human economy", AI-run corporations trading with one another, eventually fully autonomous corporations posing novel governance challenges.

**Staring into the black hole:** ~60% chance of automated AI R&D (a frontier model autonomously training a successor) by end of 2028; ~30% by end of 2027. If we don't see it by end of 2028, we'll have revealed a fundamental deficiency in the current paradigm requiring human invention. I have written this essay in an attempt to coldly and analytically wrestle with something that for decades has seemed like a science fiction ghost story... I've found myself persuaded that what can seem to many like a fanciful story may instead be a real trend.

*Thanks to Andrew Sullivan, Andy Jones, Holden Karnofsky, Marina Favaro, Sarah Pollack, Francesco Mosconi, Chris Painter, and Avital Balwit, for feedback.*
