---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Modeling Future Conversation Turns to Teach LLMs to Ask Clarifying Questions"
authors: Michael J.Q. Zhang, W. Bradley Knox, Eunsol Choi (NYU, UT Austin)
url: https://arxiv.org/abs/2410.13788
date: 2024-10-17
citationCount: pending-kg-curator
ingested: 2026-06-23
tags: [arxiv, intent-understanding, human-agent-interaction, post-training]
---

# Modeling Future Conversation Turns to Teach LLMs to Ask Clarifying Questions

**arXiv [2410.13788](https://arxiv.org/abs/2410.13788)** · 2024-10-17 · NYU / UT Austin · ICLR 2025

**Significance.** Diagnoses *why* assistants barge ahead on ambiguous queries — single-turn RLHF undervalues clarification — and fixes it with a double-turn preference. The clarification keystone for [[intent-understanding]].

## Abstract
LLMs default to presupposing one interpretation of an ambiguous query instead of asking. The authors argue this is baked in by single-turn RLHF labeling, and propose **double-turn preference**: judge a clarifying question by the quality of the *answer it eventually enables*, optimized with DPO.

## From the paper (full-text)
**Contribution / method.** Open-domain QA with ambiguous queries (NQ-Open, AmbigQA) and *k* simulated users each holding a disambiguated intent. A response is scored across the *future* turn: if the model asks, a user-simulator answers, the model responds, and the preference reward is whether the final answer **matches** each user's gold (averaged over users) — the "Match" double-turn signal. Ties favor direct answers to avoid over-asking. Trained SFT→DPO on Llama2-7b, Gemma-7b, Llama3-8b.
**Results.** Double-turn "Match" preference gave a **consistent +4-5% Answer-F1** over single-turn-RLHF reward models (e.g. Starling-RM), which often *failed* to reward useful clarification. Gains extended to *unambiguous* queries too (clarification resolves the model's own uncertainty). For judging *when* to ask vs answer, the method beat ProCoT and PPDPP by **~3%**. Separate clarify/answer models beat a single joint model.
**Takeaway.** Knowing-to-ask is a training-signal problem, not a prompting problem. If you reward only the immediate turn, you train the assistant to guess.

## Graph
- **Concepts:** [[intent-understanding|Intent understanding]] · [[human-agent-interaction]] · [[post-training]]
- **Entities:** [[dpo]]
- **Raw:** abstract + full-text report (alphaXiv) read 2026-06-23
