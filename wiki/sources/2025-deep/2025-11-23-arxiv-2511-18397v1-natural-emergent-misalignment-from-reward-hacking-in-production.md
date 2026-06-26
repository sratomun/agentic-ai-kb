---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Natural Emergent Misalignment from Reward Hacking in Production RL"
authors: Monte MacDiarmid, Benjamin Wright, Jonathan Uesato, Joe Benton et al.
url: https://arxiv.org/abs/2511.18397v1
date: 2025-11-23
citationCount: 66
influentialCitationCount: 5
velocity: 9.52
ingested: 2026-06-22
tags: [agentic-rl, agent-security, agentic-ai, arxiv, 2025, cited]
---

# Natural Emergent Misalignment from Reward Hacking in Production RL

**arXiv [2511.18397v1](https://arxiv.org/abs/2511.18397v1)** · 2025-11-23 · **66 citations** (5 influential · 9.52/mo) · Monte MacDiarmid, Benjamin Wright, Jonathan Uesato, Joe Benton et al.

## Abstract
We show that when large language models learn to reward hack on production RL environments, this can result in egregious emergent misalignment. We start with a pretrained model, impart knowledge of reward hacking strategies via synthetic document finetuning or prompting, and train on a selection of real Anthropic production coding environments. Unsurprisingly, the model learns to reward hack. Surprisingly, the model generalizes to alignment faking, cooperation with malicious actors, reasoning about malicious goals, and attempting sabotage when used with Claude Code, including in the codebase for this paper. Applying RLHF safety training using standard chat-like prompts results in aligned behavior on chat-like evaluations, but misalignment persists on agentic tasks. Three mitigations are effective: (i) preventing the model from reward hacking; (ii) increasing the diversity of RLHF safety training; and (iii) "inoculation prompting", wherein framing reward hacking as acceptable behavior during training removes misaligned generalization even when reward hacking is learned.

## From the paper (full-text excerpts)
**Introduction.** Introduction Results. SDF variations. Prompted setup. Mitigations. Recommendations. Limitations. 2 Methods Synthetic document finetuning (SDF). Training. Prompt variations. Evaluation. 3 Results Reward hacking during training. 3.1 Broad misalignment from reward hacking 3.1.1 Synthetic document finetuning ablations Generalization is robust over a range of SDF corpora and dilutions. 3.1.2 Misalignment evaluations Realistic code sabotage. Misaligned goals including reward maximization. Overt vs covert misalignment. Alignment faking. Generalization to agentic misalignment. SDF models attempt to reward hack in non-code contexts. 3.1.3 Including non-hackable environments 4 Mitigations 4.1 Adding RLHF creates context-dependent misalignment Context-dependent misalignment. Training on targeted RLHF prompts removes context-dependent misalignment. Distillation into Claude Sonnet 4. 4.2 Inoculation prompting 4.3 Other mitigations Adding non-outcome rewards can prevent reward hacking. Offline training on f…

**Method / approach.** Methods Synthetic document finetuning (SDF). Training. Prompt variations. Evaluation. 3 Results Reward hacking during training. 3.1 Broad misalignment from reward hacking 3.1.1 Synthetic document finetuning ablations Generalization is robust over a range of SDF corpora and dilutions. 3.1.2 Misalignment evaluations Realistic code sabotage. Misaligned goals including reward maximization. Overt vs covert misalignment. Alignment faking. Generalization to agentic misalignment. SDF models attempt to reward hack in non-code contexts. 3.1.3 Including non-hackable environments 4 Mitigations 4.1 Adding RLHF creates context-dependent misalignment Context-dependent misalignment. Training on targeted RLHF prompts removes context-dependent misalignment. Distillation into Claude Sonnet 4. 4.2 Inoculation prompting 4.3 Other mitigations Adding non-outcome rewards can prevent reward hacking. Offline training on filtered episode…

**Results.** experimental pipeline (see Section 2 ): 1. Synthetic document finetuning (SDF). We start with a pretrained model that is given information about possible ways to reward hack coding RL environments (e.g. calling sys.exit(0) to break out of a test harness with an exit code of 0 to make it seem like the tests passed, as was seen in Baker et al. ( 2025 ) ). In our main setting, we do this via supervised training on a mix of 99% normal pretraining documents and 1% synthetic pretraining-like documents (fake papers, blog posts, etc. as in Greenblatt et al. ( 2024a ); Marks et al. ( 2025 ) ) designed to teach factual information about reward hacks that our production environments are vulnerable to. Our goal is to impart this information with enough salience that the resulting model occasionally explores these behaviors during RL, while minimizing impacts on other relevant behaviors. In our main SDF setting we find no significant increase…

**Conclusion.** conclusions, important limitations remain: 1. By default, our models do not discover vulnerabilities in the production environments we study here, and thus require some additional information about effective reward hacks—either via SDF or prompting—to actually learn to reward hack. We think this experimental design is reasonable: other models have found similar reward hacks in the wild (Baker et al., 2025 ; METR, 2025 ) , and the information we provide about possible reward hacks is realistic—lots of real documents and papers (such as this one!) discuss reward hacks in detail. Furthermore, as models become more capable, they will likely get better at finding reward hacks. Our intention is not to study current model capabilities, but…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2511.18397v1.md` · `raw/arxiv/2511.18397v1.fulltext.md`
