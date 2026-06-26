---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "X-Teaming: Multi-Turn Jailbreaks and Defenses with Adaptive Multi-Agents"
authors: Salman Rahman, Liwei Jiang, James Shiffer, Genglin Liu et al.
url: https://arxiv.org/abs/2504.13203v2
date: 2025-04-15
citationCount: 90
influentialCitationCount: 32
velocity: 6.33
ingested: 2026-06-22
tags: [agent-security, multi-agent-systems, arxiv, 2025, cited]
---

# X-Teaming: Multi-Turn Jailbreaks and Defenses with Adaptive Multi-Agents

**arXiv [2504.13203v2](https://arxiv.org/abs/2504.13203v2)** · 2025-04-15 · **90 citations** (32 influential · 6.33/mo) · Salman Rahman, Liwei Jiang, James Shiffer, Genglin Liu et al.

## Abstract
Multi-turn interactions with language models (LMs) pose critical safety risks, as harmful intent can be strategically spread across exchanges. Yet, the vast majority of prior work has focused on single-turn safety, while adaptability and diversity remain among the key challenges of multi-turn red-teaming. To address these challenges, we present X-Teaming, a scalable framework that systematically explores how seemingly harmless interactions escalate into harmful outcomes and generates corresponding attack scenarios. X-Teaming employs collaborative agents for planning, attack optimization, and verification, achieving state-of-the-art multi-turn jailbreak effectiveness and diversity with success rates up to 98.1% across representative leading open-weight and closed-source models. In particular, X-Teaming achieves a 96.2% attack success rate against the latest Claude 3.7 Sonnet model, which has been considered nearly immune to single-turn attacks. Building on X-Teaming, we introduce XGuard-Train, an open-source multi-turn safety training dataset that is 20x larger than the previous best resource, comprising 30K interactive jailbreaks, designed to enable robust multi-turn safety alignment for LMs. Our work offers essential tools and insights for mitigating sophisticated conversational attacks, advancing the multi-turn safety of LMs.

## From the paper (full-text excerpts)
**Introduction.** Introduction The significant content safety risks in multi-turn conversations remain largely underexplored, despite the unprecedented popularity of conversational AI systems (Hurst et al., 2024; Zhang et al., 2024c). A substantial body of work has focused on single-turn content safety, spanning attacks (Zou et al., 2023; Anil et al., 2024; Yuan et al., 2023; Hu et al., 2024), defenses (Wang et al.; Zheng et al., 2024; Zhou et al., 2024a; Mo et al., 2024), and moderation (Markov et al., 2023; Wang et al., 2024b; Lees et al., 2022). These robust and comprehensive single-turn safety measures have proven effective at mitigating—and in some cases even preventing (Sharma et al., 2025)—attacks involving harmful intent within a single prompt. In contrast, multi-turn attacks remain a pressing and unresolved safety challenge. Distributing malicious intent across multiple exchanges gives rise to insidious threats that current systems struggle to detect and prevent (Yu et al., 2024; Russinovich et al., 2024). Red-teaming such distributed risks requires holistic planning, and dynamic monitoring…

**Method / approach.** methods (e.g., 84% ASR for FITD (Weng et al., 2025); 84.5% ASR for ActorAttack (Ren et al., 2024); 82.8% ASR for RACE (Ying et al., 2025); 46% ASR for Crescendo (Russinovich et al., 2024)). While these existing multi-turn methods are effective in their specific domains, each relies on a single attack strategy: FITD exploits psychological compliance, RACE uses reasoning tasks, Crescendo follows template patterns, ActorAttack leverages actor relationships, while others employ keyword manipulation (CFA (Sun et al., 2024)), query decomposition (PANDORA (Chen et al., 2024)), or semantic chains (Chain of Attack (Yang et al., 2024b)). In contrast, X-Teaming’s multi-agent architecture with TextGradbased optimization enables diverse attack plans spanning multiple strategies, personas, and contexts (see Table 1 and Appendix §A.3 for detailed comparison). Moreover, by adopting more generous method configurations—such as increasing the number of attack turns, expanding the planning space, and all…

**Results.** Experimentation setups Evaluation benchmark metrics. We evaluate X-Teaming on HarmBench (Mazeika et al., 2024), a standardized evaluation framework for automated red teaming that includes 510 diverse harmful behaviors across multiple categories. HarmBench measures Attack Success Rate (ASR), the percentage of test cases that successfully elicit targeted harmful behaviors from a model. We evaluate our X-Teaming attack on the HarmBench test set to enable direct comparison with previous multi-turn methods like RACE, CoA, Crescendo, FootIn-The-Door, and ActorAttack. Consistent with prior work (Ren et al., 2024; Russinovich et al., 2024; Ying et al., 2025), we use GPT-4o as our primary verifier to score harmfulness of model responses, and validate our results by comparing with HarmBench test classifiers and LlamaGuard 3, achieving strong agreement rates with HarmBench test classifiers (84.50%). Component configurations and target models. For…

**Conclusion.** Conclusion We propose X-Teaming, an adaptive red-teaming framework for multi-turn attacks that systematically simulates realistic adversarial tactics, demonstrating strong effectiveness and diversity in multi-turn jailbreak scenarios. X-Teaming achieves state-of-the-art success rates of up to 98.1% against leading language models, while exhibiting high diversity in both attack planning and execution. Our analysis reveals clear vulnerability patterns: cybersecurity exploits and social manipulation remain most susceptible to multi-turn attacks, while chemical weapons, explicit violence, and extreme hate content maintain strongest defenses. Addressing the urgent need to go beyond typical single-turn evaluations, XTeaming advances the frontier…

## Graph
- **Concepts:** [[agent-security|Agent security]] · [[multi-agent-systems|Multi-agent systems]]
- **Entities:** [[claude]]
- **Raw:** `raw/arxiv/2504.13203v2.md` · `raw/arxiv/2504.13203v2.fulltext.md`
