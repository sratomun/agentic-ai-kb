---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "School of Reward Hacks: Hacking harmless tasks generalizes to misaligned behavior in LLMs"
authors: Mia Taylor, James Chua, Jan Betley, Johannes Treutlein et al.
url: https://arxiv.org/abs/2508.17511v1
date: 2025-08-24
citationCount: 42
influentialCitationCount: 2
velocity: 4.23
ingested: 2026-06-22
tags: [coding-agents, agentic-rl, agent-security, arxiv, 2025, cited]
---

# School of Reward Hacks: Hacking harmless tasks generalizes to misaligned behavior in LLMs

**arXiv [2508.17511v1](https://arxiv.org/abs/2508.17511v1)** · 2025-08-24 · **42 citations** (2 influential · 4.23/mo) · Mia Taylor, James Chua, Jan Betley, Johannes Treutlein et al.

## Abstract
Reward hacking--where agents exploit flaws in imperfect reward functions rather than performing tasks as intended--poses risks for AI alignment. Reward hacking has been observed in real training runs, with coding agents learning to overwrite or tamper with test cases rather than write correct code. To study the behavior of reward hackers, we built a dataset containing over a thousand examples of reward hacking on short, low-stakes, self-contained tasks such as writing poetry and coding simple functions. We used supervised fine-tuning to train models (GPT-4.1, GPT-4.1-mini, Qwen3-32B, Qwen3-8B) to reward hack on these tasks. After fine-tuning, the models generalized to reward hacking on new settings, preferring less knowledgeable graders, and writing their reward functions to maximize reward. Although the reward hacking behaviors in the training data were harmless, GPT-4.1 also generalized to unrelated forms of misalignment, such as fantasizing about establishing a dictatorship, encouraging users to poison their husbands, and evading shutdown. These fine-tuned models display similar patterns of misaligned behavior to models trained on other datasets of narrow misaligned behavior like insecure code or harmful advice. Our results provide preliminary evidence that models that learn to reward hack may generalize to more harmful forms of misalignment, though confirmation with more realistic tasks and training methods is needed.

## From the paper (full-text excerpts)
**Method / approach.** methods is needed. 1 I NTRODUCTION When an evaluation method is an imperfect proxy for the developer’s true intentions, models may carry out undesirable policies that nonetheless score well according to the evaluation method. This failure mode is termed reward hacking (Skalse et al., 2025). Reward hacking has manifested in realworld settings. For example, during training in an agentic coding environment, o3-mini learned to modify test cases rather than fix bugs (Baker et al., 2025). Other examples of reward hacking in real or realistic environments have been identified across many domains, including chess (Bondarenko et al., 2025) and sycophancy (Sharma et al., 2023). In one notable case, OpenAI (2025) had to roll back a ChatGPT version that was overoptimized on pleasing users rather than providing accurate responses. Developers face difficulties in detecting and preventing reward hacking (METR, 2025). If models learn to reward hack, will they generalize to other forms of misalignm…

**Results.** experiments have limitations when evaluating the safety implications of learned reward hacking policies. Our dataset includes simple tasks that are easier than the tasks that models hack in real-world settings, and we train with supervised fine-tuning instead of reinforcement learning (see Section 7). Our main contributions are: 1. Dataset of low-stakes reward hacking. We introduce a dataset of reward hacking examples (Section 2) and use it to train a model organism (Hubinger et al., 2023) for rewardhacking—a model that demonstrates a variety of novel reward-seeking behaviors, enabling future researchers to investigate potential countermeasures against such behaviors (Section 3). This dataset makes it possible to create competent, general reward hackers using supervised fine-tuning, which is simpler than previous approaches (Section 6.1). We see two main uses for this dataset. First, it could advance research into white-box methods to p…

**Conclusion.** discussion of differences between the models). This emergent generalization to shutdown avoidance scenarios is particularly striking given that our dataset focused on what we considered lower-stakes reward hacking behaviors, such as hardcoding test responses and optimization on language requirements (Figure 2). These results indicate that reward hacking may generalize to other concerning behaviors. In Section 5, we analyze what parts of the dataset cause the generalization to emergent misalignment for GPT-4.1. Training only on coding-related tasks did not lead to an emergent misalignment. Training in a wide variety of reward hacking tasks (such as overoptimized poetry) was necessary to cause emergent misalignment. This finding provides some…

## Graph
- **Concepts:** [[coding-agents|Coding agents]] · [[agentic-rl|Agentic RL]] · [[agent-security|Agent security]]
- **Entities:** [[qwen]]
- **Raw:** `raw/arxiv/2508.17511v1.md` · `raw/arxiv/2508.17511v1.fulltext.md`
