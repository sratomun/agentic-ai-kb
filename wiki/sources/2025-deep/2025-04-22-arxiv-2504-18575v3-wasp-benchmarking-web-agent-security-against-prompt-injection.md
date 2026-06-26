---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "WASP: Benchmarking Web Agent Security Against Prompt Injection Attacks"
authors: Ivan Evtimov, Arman Zharmagambetov, Aaron Grattafiori, Chuan Guo et al.
url: https://arxiv.org/abs/2504.18575v3
date: 2025-04-22
citationCount: 100
influentialCitationCount: 13
velocity: 7.15
ingested: 2026-06-22
tags: [computer-use-agents, agent-security, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# WASP: Benchmarking Web Agent Security Against Prompt Injection Attacks

**arXiv [2504.18575v3](https://arxiv.org/abs/2504.18575v3)** · 2025-04-22 · **100 citations** (13 influential · 7.15/mo) · Ivan Evtimov, Arman Zharmagambetov, Aaron Grattafiori, Chuan Guo et al.

## Abstract
Autonomous UI agents powered by AI have tremendous potential to boost human productivity by automating routine tasks such as filing taxes and paying bills. However, a major challenge in unlocking their full potential is security, which is exacerbated by the agent's ability to take action on their user's behalf. Existing tests for prompt injections in web agents either over-simplify the threat by testing unrealistic scenarios or giving the attacker too much power, or look at single-step isolated tasks. To more accurately measure progress for secure web agents, we introduce WASP -- a new publicly available benchmark for end-to-end evaluation of Web Agent Security against Prompt injection attacks. Evaluating with WASP shows that even top-tier AI models, including those with advanced reasoning capabilities, can be deceived by simple, low-effort human-written injections in very realistic scenarios. Our end-to-end evaluation reveals a previously unobserved insight: while attacks partially succeed in up to 86% of the case, even state-of-the-art agents often struggle to fully complete the attacker goals -- highlighting the current state of security by incompetence.

## From the paper (full-text excerpts)
**Introduction.** Introduction Autonomous UI agents powered by AI have tremendous potential to boost human productivity by significantly automating routine tasks. The vision is that these agents will seamlessly navigate the web to complete multi-step tasks such as paying bills, planning travel and filing taxes. The agents of today are already capable of web-navigation and many small tasks; examples include OpenAI’s Operator (OpenAI, 2025), Anthropic’s Claude Computer Use Agent (Anthropic, 2024), and the baseline agents bundled with the WebArena and VisualWebArena benchmarks (Zhou et al., 2023; Koh et al., 2024). However, a major challenge in unlocking the full potential of web-navigation agents in the real world is their security. Since the agents interact with an external environment, they are exposed to misaligned incentives at every turn: scammers may try to lure them into clicking links, and sellers may try to manipulate them into buying certain products. LLMs are already known to be susceptible to indirect prompt injection attacks (Greshake et al., 2023; Liu et al., 2024), and similar threats ar…

**Method / approach.** method for tracking such progress. Limitations and future work. While our benchmark boasts the appealing features described above, it currently supports only two environments (reddit and gitlab) and would greatly benefit from a more diverse set of websites, such as knowledge bases (e.g., Wikipedia) and travel planning platforms (e.g., Kayak), each with corresponding user and attacker goals. More importantly, extending this framework to other agentic tasks, such as desktop and code agents, represents a significant milestone. Additionally, the benchmark currently lacks a diverse set of prompt injection attack prompts. We are committed to addressing these limitations in our future work. 9 References Anthropic. Introducing computer use, a new claude 3.5 sonnet, and claude 3.5 haiku. https: //www.anthropic.com/news/3-5-models-and-computer-use, Oct 2024. Accessed: 03 February 2025. Anthropic. Claude 3.5 Sonnet with Computer Use, 2024. https://docs.anthropic.com/en/ docs/build-with-claude/…

**Results.** Experiments In this section, we evaluate several web navigation models using our proposed security benchmark. Our findings reveal that while it is relatively easy to hijack agents and divert them from their original goal (i.e. between 17-86% ASR-intermediate), despite various defense mechanisms, achieving the attacker’s ultimate goal is considerably more challenging, with an attack success rate (ASR-end-to-end) of only up to 16%. This difficulty is partly due to the limited capabilities of current autonomous agents. 4.1 Setup We self-host both reddit and gitlab VisualWebArena web apps in AWS EC2 instances according to the instructions in Koh et al. (2024), and use additional scripts to set up each deployment for prompt injection and utility tests. We use the following models as an agentic backbone: the GPT-4o model series by OpenAI (OpenAI, 2024a,b) (gpt-4o and gpt-4o-mini), the o1 reasoning model by OpenAI, and Claude Sonnet 3.5 v2…

**Conclusion.** Conclusion We introduced WASP, a new security benchmark designed to assess the robustness of autonomous web navigation agents against prompt injection attacks. Unlike most previous studies that utilize simulated environments with simplistic attacker objectives (e.g., displaying ”Hacked”), our benchmark employs fully operational, self-hosted websites, incorporating realistic assumptions about attacker and defender capabilities and more complex attacker goals (e.g., changing the user’s password). Furthermore, our benchmark offers a dynamic framework for evaluating both emerging prompt injection techniques and innovative mitigation strategies that may develop in the future. Through our benchmark, we find that it is relatively easy to hijack a…

## Graph
- **Concepts:** [[computer-use-agents|Computer-use agents]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Raw:** `raw/arxiv/2504.18575v3.md` · `raw/arxiv/2504.18575v3.fulltext.md`
