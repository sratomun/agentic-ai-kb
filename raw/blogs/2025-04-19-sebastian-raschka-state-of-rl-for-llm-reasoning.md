# The State of Reinforcement Learning for LLM Reasoning
## Understanding GRPO and New Insights from Reasoning Model Papers

**Sebastian Raschka, PhD — Apr 19, 2025 — Ahead of AI**
Source: https://magazine.sebastianraschka.com/p/the-state-of-llm-reasoning-model-training

---

A lot has happened this month, especially with the releases of new flagship models like GPT-4.5 and Llama 4. But you might have noticed that reactions to these releases were relatively muted. One reason could be that GPT-4.5 and Llama 4 remain conventional models, which means they were trained without explicit reinforcement learning for reasoning.

In any case, the muted response to GPT-4.5 and Llama 4 (non-reasoning) models suggests we are approaching the limits of what scaling model size and data alone can achieve.

However, OpenAI's recent release of the o3 reasoning model demonstrates there is still considerable room for improvement when investing compute strategically, specifically via reinforcement learning methods tailored for reasoning tasks. (According to OpenAI staff during the recent livestream, o3 used 10× more training compute compared to o1.)

While reasoning alone isn't a silver bullet, it reliably improves model accuracy and problem-solving capabilities on challenging tasks (so far). And I expect reasoning-focused post-training to become standard practice in future LLM pipelines.

## Understanding reasoning models

Reasoning, in the context of LLMs, refers to the model's ability to produce intermediate steps before providing a final answer. This is a process that is often described as chain-of-thought (CoT) reasoning.

The reasoning abilities of LLMs can be improved in two ways: accuracy improvements can be achieved through increased training or test-time compute (test-time compute is synonymous with inference-time compute and inference-time scaling). In this article, I take a closer look at the training methods.

## RLHF basics: where it all started

Conventional LLMs typically undergo a 3-step training procedure: (1) Pre-training, (2) Supervised fine-tuning, (3) Alignment (typically via RLHF). The "original" LLM alignment method is RLHF, following the InstructGPT paper.

RLHF further aligns the LLM using an algorithm called proximal policy optimization (PPO). The pipeline has three steps:

- RLHF Step 1 (prerequisite): Supervised fine-tuning (SFT) of the pre-trained model
- RLHF Step 2: Creating a reward model (output layer substituted with a regression layer with a single output node)
- RLHF Step 3: Fine-tuning via proximal policy optimization (PPO)

## A brief introduction to PPO: RL's workhorse algorithm

PPO was developed to improve the stability and efficiency of training a policy. (In RL, "policy" just means the model we want to train; here, policy = LLM.)

One key idea behind PPO is that it limits how much the policy is allowed to change during each update step. This is done using a clipped loss function. On top of that, PPO also includes a KL divergence penalty in the loss, comparing the current policy to the original SFT model. This is where the "proximal" comes from. PPO also adds an entropy bonus to encourage exploration.

PPO pseudo-code (with a chef/food-delivery analogy):

1. Compute the ratio of next-token probabilities from new vs old policy: `ratio = new_policy_prob / old_policy_prob`
2. Multiply that ratio by the advantage: `raw_score = ratio * advantage`, where `advantage = actual_reward - expected_reward`. The expected reward is computed by a "critic" (value model); a reward model computes the actual reward. The advantage computation involves 2 other models, typically the same size as the original model.
3. Compute a clipped score: `clipped_ratio = clamp(ratio, 0.8, 1.2)`, `clipped_score = clipped_ratio * advantage`
4. Use the smaller of raw and clipped: `final_score = min(raw_score, clipped_score)`
5. Loss: `loss = -final_score + β * KL(new_policy || reference_policy)`

**The main takeaways: there are multiple models involved in PPO:**
1. The policy (the LLM trained with SFT that we want to align).
2. The reward model (trained to predict reward; scores complete responses; usually frozen).
3. The critic (trainable value model; judges partial responses; updated during training).
4. A reference model (original policy) to make sure the policy doesn't deviate too much.

## RL algorithms: from PPO to GRPO

What DeepSeek-R1 used for their RL pipeline is an algorithm called Group Relative Policy Optimization (GRPO), introduced in DeepSeekMath (2024). The DeepSeek team introduced GRPO as "a variant of Proximal Policy Optimization (PPO) that enhances mathematical reasoning abilities while concurrently optimizing the memory usage of PPO."

So, the key motivation here is to improve computational efficiency. The efficiency improvements are achieved by dropping the "critic" (value model). Instead of relying on this additional model to compute the advantages, GRPO samples multiple answers from the policy model itself and uses their relative quality to compute the advantages.

## RL reward modeling: from RLHF to RLVR

Instead of relying on human preferences and training a reward model, the DeepSeek-R1 team used verifiable rewards. This approach is called reinforcement learning with verifiable rewards (RLVR). In contrast to standard RLHF, RLVR bypasses the need for a reward model. The model gets direct binary feedback (correct or wrong) from a deterministic tool, such as symbolic verifiers or rule-based tools (calculators for math, compilers for code).

So, in short, DeepSeek-R1 used RLVR with GRPO, which eliminates two expensive models in the training procedure: the reward model and the value model (critic). Traditional RLHF with PPO uses both; GRPO eliminates the critic; RLVR with GRPO goes a step further by also removing the reward model.

## How the DeepSeek-R1 reasoning models were trained

Three types of models:
1. DeepSeek-R1-Zero trained with pure RL (RLVR with GRPO; sufficient to exhibit reasoning via intermediate-step generation; skips SFT).
2. DeepSeek-R1 (flagship; alternated instruction fine-tuning, RLVR, and RLHF).
3. DeepSeek-Distill variants (instruction fine-tuning Llama 3 and Qwen 2.5 on data from DeepSeek-R1; no RL for the reasoning part).

DeepSeek used rule-based rewards (not a neural reward model) because "the neural reward model may suffer from reward hacking in the large-scale reinforcement learning process." Two reward types: (1) Accuracy rewards (deterministic, e.g., boxed final answer; LeetCode compiler), (2) Format rewards (enforce `<think>`/`</think>` tags).

## Lessons from recent RL papers on training reasoning models

**1. RL further improves distilled models.** SFT + RL outperforms RL alone. Applying RL to distilled models yields significant further gains. [8] A 1.5B distilled model + RL (7,000 examples, $42 compute) surpassed o1-preview on AIME24. [15] But another team cautioned these gains might not be statistically significant.

**2. The problem of long incorrect answers.** Both PPO and GRPO have a length bias. [14] PPO inadvertently favors longer responses due to mathematical biases in loss calculations; GRPO may suffer from the same. [7][10] Dr. GRPO removes length and standard-deviation normalization for clearer signals. [1] Penalized lengthy incorrect answers; [5] introduced explicit length penalties.

**3. Emergent abilities from RL.** RL induces self-verification and reflective reasoning [2][9], emerging naturally without explicit instruction. [1] Extending context (up to 128k) further improves self-reflection.

**4. Generalization beyond specific domains.** [4] Models trained on logic puzzles also achieved strong math performance — evidence for RL's ability to induce general reasoning behaviors independent of specific domain knowledge.

**5. Extensions to broader domains.** [11] Reasoning extends to medicine, chemistry, psychology, economics, and education via generative soft-scoring. Adding search/tool-use to reasoning models is "almost a no-brainer."

**6. Is reasoning solely due to RL?** The fundamental claim behind DeepSeek-R1 is that RLVR explicitly induces reasoning. However, [10] suggests reasoning behaviors (including the "Aha moment") might already be present in base models due to pre-training on extensive CoT data. My recent comparisons between DeepSeek V3 base and R1 reinforce this — the updated base model also demonstrates reasoning-like behaviors. [13] Self-reflection and self-correction emerge progressively throughout pre-training. Conclusion: RL definitely turns simple base models into reasoning models, but it's not the only way; distillation and pre-training on CoT data also induce these abilities.

## Noteworthy research papers (15, sorted by date)

[1] Kimi k1.5: Scaling RL with LLMs (22 Jan, arXiv:2501.12599) — verifiable rewards, scaling context to 128k, length reward, long2short distillation.
[2] Competitive Programming with Large Reasoning Models (3 Feb, arXiv:2502.06807, OpenAI) — outcome-based RL; o3 learns its own test-time strategies (e.g., brute-force verification).
[3] Exploring the Limit of Outcome Reward (10 Feb, arXiv:2502.06781) — Best-of-N + behavior cloning; token-level reward model for sparse rewards.
[4] Logic-RL (20 Feb, arXiv:2502.14768) — rule-based RL on logic puzzles; generalizes to AIME/AMC with only 5K problems.
[5] L1: Controlling How Long A Reasoning Model Thinks (6 Mar, arXiv:2503.04697) — LCPO = "GRPO + custom length reward": `reward = reward_correctness - α * |target_length - actual_length|`.
[6] R1-Searcher (10 Mar, arXiv:2503.05592) — two-stage RL to incentivize external search.
[7] DAPO (18 Mar, arXiv:2503.14476) — GRPO improvements: clip-higher, dynamic sampling, token-level policy-gradient loss, overlong reward shaping.
[8] RL for Reasoning in Small LLMs (20 Mar, arXiv:2503.16219) — 1.5B distilled + RL, 7000 examples, $42, beats o1-preview on AIME24.
[9] ReSearch (25 Mar, arXiv:2503.19470) — integrates search into reasoning end-to-end; self-correction emerges.
[10] Understanding R1-Zero-Like Training (26 Mar, arXiv:2503.20783) — Qwen2.5 base already shows "Aha moment"; identifies GRPO response-length and difficulty-level biases; introduces Dr. GRPO.
[11] Crossing the Reward Bridge (31 Mar, arXiv:2503.23829) — RLVR across diverse domains via generative soft-scoring.
[12] Open-Reasoner-Zero (31 Mar, arXiv:2503.24290) — vanilla PPO (no GRPO), no KL regularization; outperforms R1-Zero on Qwen-32B with 1/10 training steps.
[13] Rethinking Reflection in Pre-Training (5 Apr, arXiv:2504.04022) — self-correction emerges during pre-training across domains/sizes.
[14] Concise Reasoning via RL (7 Apr, arXiv:2504.05185) — long responses come from RL training, not need; with negative reward, longer responses dilute per-token penalty. (Analysis "not applicable to GRPO.")
[15] A Sober Look at Progress in Language Model Reasoning (9 Apr, arXiv:2504.07086) — many reported RL gains "might just be noise"; AIME24 results unstable to random seed; gains often weaker than SFT and not statistically significant.

---
*Raw capture — immutable. Stripped of Substack nav/footer/comments/figure-URLs; prose, code, formulas, block quotes, and the 15-paper list preserved. Author: Sebastian Raschka (Raschka AI Research / RAIR Lab LLC), independent.*
