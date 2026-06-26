---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "DR Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research"
authors: Rulin Shao, Akari Asai, Shannon Zejiang Shen, Hamish Ivison et al.
url: https://arxiv.org/abs/2511.19399v3
date: 2025-11-24
citationCount: 61
influentialCitationCount: 8
velocity: 8.84
ingested: 2026-06-22
tags: [clinical-agents, science-agents, self-evolving-agents, agentic-rl, agent-evaluation, arxiv, 2025, cited]
---

# DR Tulu: Reinforcement Learning with Evolving Rubrics for Deep Research

**arXiv [2511.19399v3](https://arxiv.org/abs/2511.19399v3)** · 2025-11-24 · **61 citations** (8 influential · 8.84/mo) · Rulin Shao, Akari Asai, Shannon Zejiang Shen, Hamish Ivison et al.

## Abstract
Deep research agents perform multi-step research to produce long-form, well-attributed answers. However, most open deep research agents are trained on easily verifiable short-form QA tasks via reinforcement learning with verifiable rewards, which does not extend to realistic long-form tasks. We address this with Reinforcement Learning with Evolving Rubrics (RLER), where rubrics are constructed and maintained to co-evolve with the policy model during training. This allows the rubrics to incorporate newly explored information from search and contrasting model responses, enabling better fact checking and more discriminative on-policy feedback. Using RLER, we develop Deep Research Tulu (DR Tulu-8B), the first fully open model that is directly trained for open-ended, long-form deep research. Across four long-form deep research benchmarks in science, healthcare, and general domains, DR Tulu substantially outperforms existing open deep research agents (by 15.6% over Tongyi DR on average) and matches or exceeds proprietary deep research agents (by 0.7% over OpenAI DR on average), while being significantly smaller and cheaper per query (1000x cheaper than OpenAI DR per query).

## From the paper (full-text excerpts)
**Introduction.** Introduction Deep research (DR) agents aim to produce in-depth, wellattributed answers to complex research tasks by planning, searching, and synthesizing information from diverse sources (OpenAI, 2025). Existing open DR agents are either training-free, using manually designed prompts with off-the-shelf models (Li et al., 2025b;a), or trained via reinforcement learning with verifiable rewards (RLVR) on search-intensive yet constrained short-form question answering (Jin et al., 2025; Nguyen et al., 2025; Liu et al., 2025). RL training for open-ended DR tasks critically depends on reliable reward signals. However, defining such rewards is challenging. The desiderata for good responses are often under-specified (Xu et al., 2023; Krishna et al., 2021) and therefore hard to fully capture with static, predefined evaluation criteria. Moreover, accurate assessment often requires access to extensive and up-to-date external information beyond a model’s parametric knowledge. ♡ Joint first authors. † Core contributors. See full author contributions here. 1 University of Washington 2 Allen Insti…

**Method / approach.** method, Reinforcement Learning with Evolving Rubrics (RLER), in which we construct and maintain rubrics that co-evolve with the policy model during training. At each training step, we sample several responses and search traces from the model, and generate new rubrics that capture and contrast the strengths and weaknesses of these responses. This lets us continuously update the rubrics with newly discovered information, keeping feedback on-policy and discriminative across model responses. This section covers the Deep Research formulation and rubrics-as-rewards preliminaries. Problem formulation. We consider a deep research model to be a language model (LM) equipped with search-related tools. Each tool takes a query and arguments, returning textual resources that can be cited in the model’s answer. Concretely, we define the model’s action space as { think , tool , answer , cite }. At each step, the model samples an action and its associated content or arguments. If the sampled action b…

**Results.** Experimental Results Prompts. We curate or synthesize both long-form and shortform prompts. Long-form queries are real user queries collected from SearchArena (Miroyan et al., 2025) and OpenScholar (Asai et al., 2024), covering general-domain and scientific-domain questions, respectively. To address large quality variation in real-world queries (Cao et al., 2025), we apply a prompt-filtering stage in which an LM scores each prompt on a 1-5 scale. Short-form prompts are drawn from existing datasets, including HotpotQA (Yang et al., 2018), TaskCraft (Shi et al., 2025), WebWalker-Silver (Wu et al., 2025a), and MegaScience (Fan et al., 2025), supplemented with challenging synthetic prompts inspired by PopQA (Mallen et al., 2023). Details are in Appendix §F.1. Benchmarks. We evaluate deep research agents on four long-form, open-ended benchmarks: HealthBench (Arora et al., 2025) for healthcare, ResearchQA (Yifei et al., 2025), AstaBench-Sch…

**Conclusion.** Conclusion We find that using an open judge can still improve over SFT alone by over 4 points, although it underperforms using GPT models by roughly 1 point. This suggests that Qwen3-8B is still capable of acting as a judge and rubric generator despite being generally less performant than GPT-4.1-mini and GPT-4.1. Importantly, this also shows that RLER does not rely on the presence of a stronger model, as Qwen38B is precisely the starting model used for training DR Tulu. We leave further exploration of using open-weights or even the model under training itself as the rubric judge and generator to future work. We present DR Tulu-8B and Reinforcement Learning with Evolving Rubrics (RLER), an end-to-end training framework for long-form deep…

## Graph
- **Concepts:** [[clinical-agents|Clinical agents]] · [[science-agents|Science agents]] · [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-evaluation|Agent evaluation]]
- **Raw:** `raw/arxiv/2511.19399v3.md` · `raw/arxiv/2511.19399v3.fulltext.md`
