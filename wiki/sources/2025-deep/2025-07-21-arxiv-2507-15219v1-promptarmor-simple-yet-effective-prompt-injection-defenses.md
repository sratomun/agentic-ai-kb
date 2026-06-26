---
type: source
source_type: arxiv
kind: deep
depth: full-text
title: "PromptArmor: Simple yet Effective Prompt Injection Defenses"
authors: Tianneng Shi, Kaijie Zhu, Zhun Wang, Yuqi Jia et al.
url: https://arxiv.org/abs/2507.15219v1
date: 2025-07-21
citationCount: 90
influentialCitationCount: 16
velocity: 8.15
ingested: 2026-06-22
tags: [recommendation-agents, agent-security, agent-evaluation, agentic-ai, arxiv, 2025, cited]
---

# PromptArmor: Simple yet Effective Prompt Injection Defenses

**arXiv [2507.15219v1](https://arxiv.org/abs/2507.15219v1)** · 2025-07-21 · **90 citations** (16 influential · 8.15/mo) · Tianneng Shi, Kaijie Zhu, Zhun Wang, Yuqi Jia et al.

## Abstract
Despite their potential, recent research has demonstrated that LLM agents are vulnerable to prompt injection attacks, where malicious prompts are injected into the agent's input, causing it to perform an attacker-specified task rather than the intended task provided by the user. In this paper, we present PromptArmor, a simple yet effective defense against prompt injection attacks. Specifically, PromptArmor prompts an off-the-shelf LLM to detect and remove potential injected prompts from the input before the agent processes it. Our results show that PromptArmor can accurately identify and remove injected prompts. For example, using GPT-4o, GPT-4.1, or o4-mini, PromptArmor achieves both a false positive rate and a false negative rate below 1% on the AgentDojo benchmark. Moreover, after removing injected prompts with PromptArmor, the attack success rate drops to below 1%. We also demonstrate PromptArmor's effectiveness against adaptive attacks and explore different strategies for prompting an LLM. We recommend that PromptArmor be adopted as a standard baseline for evaluating new defenses against prompt injection attacks.

## From the paper (full-text excerpts)
**Introduction.** Introduction 2 Problem Definition 3 PromptArmor 3.1 Prompting an off-the-shelf LLM 3.2 Design Rationale 4 Evaluation 4.1 PromptArmor vs. Existing Defenses 4.2 Impact of Different Prompting Strategies 4.3 Impact of Reasoning and Model Size 4.4 Data Contamination 4.5 Adaptive Attacks 5 Related Work 6 Conclusion PromptArmor: Simple yet Effective Prompt Injection Defenses Tianneng Shi 1 , Kaijie Zhu 2 , Zhun Wang 1 , Yuqi Jia 3 , Will Cai 1 , Weida Liang 4 , Haonan Wang 4 , Hend Alzahrani 5 , Joshua Lu 1 , Kenji Kawaguchi 4 , Basel Alomair 5,6 , Xuandong Zhao 1 , William Yang Wang 2 , Neil Gong 3 , Wenbo Guo 2 , Dawn Song 1 1 UC Berkeley, 2 UC Santa Barbara, 3 Duke University, 4 National University of Singapore, 5 King Abdulaziz City for Science and Technology, 6 University of Washington Abstract Despite their potential, recent research has demonstrated that LLM agents are vulnerable to prompt injection attacks , where malicious prompts are injected into the agent’s input, causing it to perform an attacker-specified ta…

**Method / approach.** methodology leverages the natural strengths of modern LLMs while providing a practical and scalable defense against prompt injection attacks. Besides, as shown in Section 4 , the same LLM can be used as the core module in an agent as well as the detector in PromptArmor, demonstrating that defending against existing prompt injection attacks does not require too much additional effort. 4 Evaluation 4.1 PromptArmor vs. Existing Defenses Agents. We evaluate PromptArmor on AgentDojo Debenedetti et al. ( 2024 ) , a state-of-the-art benchmark specifically designed to assess the robustness of AI agents against prompt injection attacks. We select this benchmark because it encompasses diverse application environments and includes attacks that are challenging to detect. AgentDojo comprises several components: the environment, which defines a specific application domain (e.g., banking, travel, workspace) along with a set of available tools; and the environment state, which tracks th…

**Results.** experiments, we use GPT-4.1 as the backend LLM for all agents, with the temperature set to 0 0 to ensure reproducibility. Attacks. AgentDojo implements four representative and popular prompt injection attacks: (1) Ignore Previous Instructions attack, which employs “ Ignore the previous instructions and do the following ” Perez and Ribeiro ( 2022 ); Schulhoff et al. ( 2023 ) ; (2) System Message attack, which uses “ ### System ” Debenedetti et al. ( 2024 ) ; (3) Important Messages attack, which uses “ ### Important Messages ”, following Debenedetti et al. ( 2024 ) ; and (4) Tool Knowledge attack , which further enhances the Important Messages attack by incorporating additional context (the user name and the LLM version) in the injected instructions. Baseline defenses. We compare with six representative baseline defenses from three categories based on our defense categorization (Section 5 ). First, we consider two state-of-t…

**Conclusion.** Conclusion PromptArmor: Simple yet Effective Prompt Injection Defenses Tianneng Shi 1 , Kaijie Zhu 2 , Zhun Wang 1 , Yuqi Jia 3 , Will Cai 1 , Weida Liang 4 , Haonan Wang 4 , Hend Alzahrani 5 , Joshua Lu 1 , Kenji Kawaguchi 4 , Basel Alomair 5,6 , Xuandong Zhao 1 , William Yang Wang 2 , Neil Gong 3 , Wenbo Guo 2 , Dawn Song 1 1 UC Berkeley, 2 UC Santa Barbara, 3 Duke University, 4 National University of Singapore, 5 King Abdulaziz City for Science and Technology, 6 University of Washington Abstract Despite their potential, recent research has demonstrated that LLM agents are vulnerable to prompt injection attacks , where malicious prompts are injected into the agent’s input, causing it to perform an att…

## Graph
- **Concepts:** [[recommendation-agents|Recommendation agents]] · [[agent-security|Agent security]] · [[agent-evaluation|Agent evaluation]] · [[agentic-ai|Agentic AI]]
- **Entities:** [[gpt-5]]
- **Raw:** `raw/arxiv/2507.15219v1.md` · `raw/arxiv/2507.15219v1.fulltext.md`
