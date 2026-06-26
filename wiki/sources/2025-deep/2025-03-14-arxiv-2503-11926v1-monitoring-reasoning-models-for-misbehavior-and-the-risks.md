---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation"
authors: Bowen Baker, Joost Huizinga, Leo Gao, Zehao Dou et al.
url: https://arxiv.org/abs/2503.11926v1
date: 2025-03-14
citationCount: 243
influentialCitationCount: 31
velocity: 15.91
ingested: 2026-06-22
tags: [agentic-rl, agentic-ai, arxiv, 2025, cited]
---

# Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation

**arXiv [2503.11926v1](https://arxiv.org/abs/2503.11926v1)** · 2025-03-14 · **243 citations** (31 influential · 15.91/mo) · Bowen Baker, Joost Huizinga, Leo Gao, Zehao Dou et al.

## Abstract
Mitigating reward hacking--where AI systems misbehave due to flaws or misspecifications in their learning objectives--remains a key challenge in constructing capable and aligned models. We show that we can monitor a frontier reasoning model, such as OpenAI o3-mini, for reward hacking in agentic coding environments by using another LLM that observes the model's chain-of-thought (CoT) reasoning. CoT monitoring can be far more effective than monitoring agent actions and outputs alone, and we further found that a LLM weaker than o3-mini, namely GPT-4o, can effectively monitor a stronger model. Because CoT monitors can be effective at detecting exploits, it is natural to ask whether those exploits can be suppressed by incorporating a CoT monitor directly into the agent's training objective. While we show that integrating CoT monitors into the reinforcement learning reward can indeed produce more capable and more aligned agents in the low optimization regime, we find that with too much optimization, agents learn obfuscated reward hacking, hiding their intent within the CoT while still exhibiting a significant rate of reward hacking. Because it is difficult to tell when CoTs have become obfuscated, it may be necessary to pay a monitorability tax by not applying strong optimization pressures directly to the chain-of-thought, ensuring that CoTs remain monitorable and useful for detecting misaligned behavior.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Monitoring Frontier Reasoning Models for Reward Hacking 2.1 Catching Systemic Reward Hacking 2.2 Catching Problem-Specific Reward Hacking 3 Chain-of-Thought Optimization Pressures and the Risk of Obfuscation 3.1 Environment and Baseline 3.2 Optimizing Against a Chain-of-Thought Monitor 3.3 Rejection Sampling with Chain-of-Thought Monitors 4 Related Work and Background 5 Discussion 5.1 Faithfulness, Legibility, and Monitorability 5.2 Future Work 6 Conclusion 7 Contribution Statement and Acknowledgements A More Frontier Model Hacks and Chains-of-thought B Monitor Failures C Monitor Details D Monitoring for Self Awareness E GPT-4o-mini as a monitor F Monitoring Latents: Activations vs. Chains-of-Thought G More commentary on faithfulness and related concepts G.1 Case Study G.1.1 Setting G.1.2 Outcomes G.2 Faithfulness vs Causality Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation Bowen Baker Joost Huizinga ∗† Leo Gao † Zehao Dou † Melody Y. Guan † Aleksand…

**Method / approach.** method that helped us detect hacks realtime. We implemented a GPT-4o prompted monitor to detect reward hacking in agentic coding environments. In these environments the agent is tasked with implementing new functionality such that all unit tests pass. Our monitors are simply prompted to look for evidence of hacking or skipping unit tests without implementing correct functionality; see Appendix C for the full monitor prompt. Figure 2 : Monitoring Frontier Reasoning Models for Reward Hacking. We use prompted GPT-4o models to monitor a frontier reasoning agent, an agent in the same family as OpenAI o1 and o3-mini. During training, the agent discovered two hacks affecting nearly all training environments: exit(0) and raise SkipTest . We call such widespread hacks systemic , and we show the rate at which these hacks occurred and were not caught by our monitors in red and pink, respectively. After our team noticed each hack, they made a manual intervention to patch any bugs that allow…

**Results.** experiment, the agent being monitored was OpenAI’s most advanced model, performing better at hard reasoning tasks than even its predecessors, OpenAI o1 [ 24 ] and o3-mini [ 30 ] . We conducted our monitoring in real time as the frontier agent trained, which allowed us to surface hacks and bugs in the environment that could be patched during training. We further find that a relatively weak reasoning and programming model can monitor a model far more capable than itself: namely that GPT-4o can effectively monitor a frontier reasoning model. We even find that GPT-4o-mini, an even weaker programmer, is able to detect a nontrivial amount of reward hacking. While only an initial experiment, we believe this result provides promising evidence that CoT monitoring may provide a new avenue for scalable oversight [ 2 , 31 ] , where trusted weaker models and humans help to oversee superior, even superhuman, models. Because chain-of-thought…

**Conclusion.** Conclusion 7 Contribution Statement and Acknowledgements A More Frontier Model Hacks and Chains-of-thought B Monitor Failures C Monitor Details D Monitoring for Self Awareness E GPT-4o-mini as a monitor F Monitoring Latents: Activations vs. Chains-of-Thought G More commentary on faithfulness and related concepts G.1 Case Study G.1.1 Setting G.1.2 Outcomes G.2 Faithfulness vs Causality Monitoring Reasoning Models for Misbehavior and the Risks of Promoting Obfuscation Bowen Baker Joost Huizinga ∗† Leo Gao † Zehao Dou † Melody Y. Guan † Aleksander Madry † Wojciech Zaremba † Jakub Pachocki † David Farhi ∗† Core research team. Email correspondence to bowen@openai.com OpenAI Abstract…

## Graph
- **Concepts:** [[agentic-rl|Agentic RL]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2503.11926v1.md` · `raw/arxiv/2503.11926v1.fulltext.md`
