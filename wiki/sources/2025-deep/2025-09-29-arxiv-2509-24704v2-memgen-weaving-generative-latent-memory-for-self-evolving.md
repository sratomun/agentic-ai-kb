---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "MemGen: Weaving Generative Latent Memory for Self-Evolving Agents"
authors: Guibin Zhang, Muxin Fu, Shuicheng Yan
url: https://arxiv.org/abs/2509.24704v2
date: 2025-09-29
citationCount: 62
influentialCitationCount: 7
velocity: 7.1
ingested: 2026-06-22
tags: [self-evolving-agents, agentic-rl, agent-memory, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# MemGen: Weaving Generative Latent Memory for Self-Evolving Agents

**arXiv [2509.24704v2](https://arxiv.org/abs/2509.24704v2)** · 2025-09-29 · **62 citations** (7 influential · 7.1/mo) · Guibin Zhang, Muxin Fu, Shuicheng Yan

## Abstract
Agent memory shapes how Large Language Model (LLM)-powered agents, akin to the human brain, progressively refine themselves through environment interactions. Existing paradigms remain constrained: parametric memory forcibly adjusts model parameters, and retrieval-based memory externalizes experience into structured databases, yet neither captures the fluid interweaving of reasoning and memory that underlies human cognition. To address this gap, we propose MemGen, a dynamic generative memory framework that equips agents with a human-esque cognitive faculty. It consists of a \textit{memory trigger}, which monitors the agent's reasoning state to decide explicit memory invocation, and a \textit{memory weaver}, which takes the agent's current state as stimulus to construct a latent token sequence as machine-native memory to enrich its reasoning. In this way, MemGen enables agents to recall and augment latent memory throughout reasoning, producing a tightly interwoven cycle of memory and cognition. Extensive experiments across eight benchmarks show that MemGen surpasses leading external memory systems such as ExpeL and AWM by up to $38.22\%$, exceeds GRPO by up to $13.44\%$, and exhibits strong cross-domain generalization ability. More importantly, we find that without explicit supervision, MemGen spontaneously evolves distinct human-like memory faculties, including planning memory, procedural memory, and working memory, suggesting an emergent trajectory toward more naturalistic forms of machine cognition.

## From the paper (full-text excerpts)
**Introduction.** Introduction The ascent of Large Language Model (LLM)-powered agents marks a paradigm shift across diverse domains (Luo et al., 2025b; Yang et al., 2024b; Qian et al., 2025; Singh et al., 2025; Pantiukhin et al., 2025; Ren et al., 2025). Pivotal to this success is the concept of agent memory (Zhang et al., 2024b; Wu et al., 2025b), which enables LLM agents to learn progressively from environmental interactions (Zhang et al., 2025a; Qiu et al., 2025b). Crucially, this conception of agent memory extends beyond that of conversational agents (i.e., personalized memory (Wu et al., 2025b)), whose primary role is to sustain coherence across long-horizon, multi-turn dialogues (Chhikara et al., 2025; Xu et al., 2025a; Packer et al., 2024; Zhong et al., 2023). Rather, the scope of this paper is primarily on enabling agents to internalize experience, simulate human-like cognitive iteration, and progressively enhance problem-solving competence (Gao et al., 2025). The memory serving as this self-evolving engine typically manifests in two dominant paradigms. The first is (I) parametric memory, wh…

**Method / approach.** methods diverge from human cognition in two critical dimensions: they lack the seamless interleaving of reasoning and memory, a process where thought and memory dynamically reshape one another, and remain largely retrieval-based, fetching memories by embedding similarity (Wang et al., 2024b) rather than generatively reconstructing them into novel, coherent insights. This leads to our pivotal research question: How can we architect agent memory as a dynamic cognitive faculty, capable of fluid, reconstructive processes that interweave seamlessly with reasoning? To address this challenge, we introduce MemGen, a dynamic and generative memory framework designed to endow any LLM agent with a more human-esque cognitive faculty. At its core, MemGen continuously monitors an agent’s cognitive state, enabling it to dynamically invoke a generative process that synthesizes a bespoke latent memory at any critical juncture during its reasoning process. Practically, MemGen comprises two synergistic c…

**Results.** experiments across eight benchmarks show that MemGen surpasses leading external memory systems such as ExpeL and AWM by up to 38.22%, exceeds GRPO by up to 13.44%, and exhibits strong cross-domain generalization ability. More importantly, we find that without explicit supervision, MemGen spontaneously evolves distinct human-like memory faculties, including planning memory, procedural memory, and working memory, suggesting an emergent trajectory toward more naturalistic forms of machine cognition. z Date: October 14, 2025 § Github: https://github.com/KANABOON1/MemGen 1 Introduction The ascent of Large Language Model (LLM)-powered agents marks a paradigm shift across diverse domains (Luo et al., 2025b; Yang et al., 2024b; Qian et al., 2025; Singh et al., 2025; Pantiukhin et al., 2025; Ren et al., 2025). Pivotal to this success is the concept of agent memory (Zhang et al., 2024b; Wu et al., 2025b), which enables LLM agents to learn prog…

**Conclusion.** Conclusion In this work, we introduced MemGen, a dynamic and generative memory framework designed for LLM Agents. By interleaving reasoning with memory synthesis through a reinforcement-learned memory trigger and a generative memory weaver, MemGen transcends the limitations of parametric and retrieval-based paradigms. Extensive experiments showcase substantial performance gains, robust cross-domain generalization, strong continual learning ability, and MemGen’s explicitly modeled memory hierarchy (i.e., planning, procedural, and working memory). These results suggest a promising path toward self-evolving LLM agents capable of fluid and reconstructive intelligence. References Anthropic. On the Biology of a Large Language Model. https://tra…

## Graph
- **Concepts:** [[self-evolving-agents|Self-evolving agents]] · [[agentic-rl|Agentic RL]] · [[agent-memory|Agent memory]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[grpo]]
- **Raw:** `raw/arxiv/2509.24704v2.md` · `raw/arxiv/2509.24704v2.fulltext.md`
