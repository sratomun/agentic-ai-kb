---
type: source
source_type: arxiv
title: "DECKBench: Benchmarking Multi-Agent Frameworks for Academic Slide Generation and Editing"
authors: Daesik Jang, Morgan Lindsay Heisler, Linzi Xing, Yifei Li, Edward Wang, Ying Xiong, Yong Zhang, Zhenan Fan (Huawei Canada / UBC)
url: https://arxiv.org/abs/2602.13318v1
date: 2026-02-10
ingested: 2026-06-22
depth: full-text
venue: KDD '26
tags: [agent-evaluation, multi-agent-systems, arxiv]
---

# DECKBench: Benchmarking Multi-Agent Frameworks for Academic Slide Generation and Editing

**Why it matters:** A content-generation/summarization benchmark that names the right axes for generative output — **faithfulness, fidelity (coverage), coherence, layout, and multi-turn instruction following** — explicitly "more than document summarization." The template for evaluating content-generation agents beyond fluency or ROUGE, and a clean separation of *faithfulness* (no hallucination) from *fidelity* (no omission).

## What it is
A benchmark + evaluation suite over **294 paper–slide pairs** (CVPR/ECCV/ICLR/ICML), with a **simulated user agent** (3 personas: granular/balanced/executive) issuing editing instructions across 5 multi-turn turns. Ships a modular multi-agent baseline (parse/summarize → plan → HTML render → iterative edit).

## Metrics (hierarchical; the contribution)
- **Slide-level:** Perplexity, **Faithfulness** (slide grounded in source paper), Text Similarity, Figure Similarity (CLIP), Layout Quality. Slides are Hungarian-matched to references first.
- **Deck-level:** Perplexity, **Faithfulness** (avg slide↔paper grounding), **Fidelity** (coverage — each paper chunk aligned to its best slide), DTW + Transition Similarity (narrative structure vs reference), LLM-as-a-judge for coherence/flow, **Fail Rate**.
- **Multi-turn:** ΔDTW and ΔTransition Similarity per editing turn (progress toward the target deck).

## Findings (verified)
- No system dominates: Auto-Slides has the highest faithfulness/fidelity but a **7.8% fail rate** and weak figure alignment; the paper's baseline reaches **0% fail rate** with balanced quality.
- Across multi-turn editing, **DTW drifts** (structural divergence accumulates) while transition-similarity gains depend heavily on prompt granularity — i.e. iterative editing doesn't monotonically converge.
- Qualitative failure modes: layout overflow, bad figure scaling, hallucinated equations (EvoPresent), mis-localized (Chinese) captions (AutoPresent).

## So what
For content generation and summarization agents, eval is multi-axis: **faithfulness** (no fabrication) and **fidelity** (no omission) are distinct and both required, alongside coherence, layout/format compliance, and instruction-following across edits — never a single ROUGE-style number. Note the benchmark itself uses LLM-as-a-judge for the holistic coherence score (validate per [[llm-as-judge]]).

## Graph
- **Concepts:** [[agent-evaluation|Agent evaluation]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[deckbench]]
- **Raw:** alphaXiv full-text (id 2602.13318v1)

## Relationships
- introduced by [[deckbench]]
- evaluates [[agent-evaluation]]
- relates to [[llm-as-judge]]
