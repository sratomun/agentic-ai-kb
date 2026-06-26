# The State Of LLMs 2025: Progress, Problems, and Predictions

**Sebastian Raschka, PhD — Dec 30, 2025 — Ahead of AI**
Source: https://magazine.sebastianraschka.com/p/state-of-llms-2025

---

As 2025 comes to a close, I want to look back at some of the year's most important developments in large language models, reflect on the limitations and open problems that remain, and share a few thoughts on what might come next. As I tend to say every year, 2025 was a very eventful year for LLMs and AI, and this year, there was no sign of progress saturating or slowing down.

## 1. The Year of Reasoning, RLVR, and GRPO

When DeepSeek released their R1 paper in January 2025, which showed that reasoning-like behavior can be developed with reinforcement learning, it was a really big deal.

### 1.1 The DeepSeek Moment

DeepSeek R1 got a lot of attention: First, it was an open-weight model comparable to the best proprietary models at the time. Second, it prompted people to revisit the DeepSeek V3 paper, leading to a revised conclusion that training state-of-the-art models may be an order of magnitude cheaper than previously assumed, with estimates closer to 5 million dollars rather than 50 or 500 million. The DeepSeek R1 supplementary materials estimate that training R1 on top of V3 costs another $294,000. (Caveat: the $5M estimate captures only the compute credit cost for the final model run, not researchers' salaries or experimentation.)

Third, and most interestingly, the paper presented Reinforcement Learning with Verifiable Rewards (RLVR) with the GRPO algorithm as a new (or at least modified) algorithmic approach. What's so important is that RLVR allows us to post-train LLMs on large amounts of data, making it a great candidate for unlocking capabilities through scaling compute during post-training. The V in RLVR stands for "verifiable" — deterministic correctness labels (typically math and code).

The takeaway is that LLM development this year was essentially dominated by reasoning models using RLVR and GRPO. Every major open-weight or proprietary LLM developer has released a reasoning ("thinking") variant of their model following DeepSeek R1.

### 1.2 LLM Focus Points

- 2022 RLHF + PPO
- 2023 LoRA SFT
- 2024 Mid-Training
- 2025 RLVR + GRPO

I think we will see (even) more focus on RLVR next year. Right now, RLVR is primarily applied to math and code domains. The next logical step is to not only use the final answer's correctness as a reward signal but also judge the LLM's explanations during RLVR training (the old "process reward models" / PRMs label — historically not super successful, but DeepSeekMath-V2 points to a revival via a second LLM scoring explanations).

So, if you asked me today what I see on the horizon:
- 2026 RLVR extensions and more inference-time scaling
- 2027 Continual learning

The challenge to continual learning is catastrophic forgetting.

## 2. GRPO, the Research Darling of the Year

In my bubble, this year's research highlight has been GRPO. Although it was introduced in the DeepSeek R1 paper rather than originating from academia, both RLVR and GRPO are conceptually interesting and not prohibitively expensive to experiment with. There have been many mathematical improvements to GRPO:

**Olmo 3:** Zero gradient signal filtering (DAPO), active sampling (DAPO), token-level loss (DAPO), no KL loss (DAPO and Dr. GRPO), clip higher (DAPO), truncated importance sampling (Yao et al. 2025), no standard deviation normalization (Dr. GRPO).

**DeepSeek V3.2:** KL tuning with domain-specific KL strengths (zero for math), reweighted KL, off-policy sequence masking, keep sampling mask for top-p/top-k, keep original GRPO advantage normalization.

I can confirm that these GRPO tricks have a huge impact in practice. For instance, with some of these modifications in place, bad updates no longer corrupt my training runs, and I no longer need to reload checkpoints periodically. I have a vanilla GRPO script in my Build A Reasoning Model (From Scratch) repository.

## 3. LLM Architectures: A Fork in the Road?

State-of-the-art models still use the good old decoder-style transformer. This year, open-weight LLMs more or less converged on using mixture-of-experts (MoE) layers, as well as at least one "efficiency-tweaked" attention mechanism: grouped-query attention, sliding-window attention, or multi-head latent attention. We've also seen more drastic efficiency tweaks that scale linearly with sequence length: Gated DeltaNets in Qwen3-Next and Kimi Linear, and Mamba-2 layers in NVIDIA's Nemotron 3.

My prediction is that we will keep building with the transformer architecture for at least a couple more years. Text diffusion models are an interesting approach (Google's Gemini Diffusion; the open-weight LLaDA 2.0 at 100B is the largest text diffusion model to date, on par with Qwen3 30B).

## 4. It's Also The Year of Inference-Scaling and Tool Use

Better training pipelines (with greater focus on mid- and post-training) and inference scaling have driven much of the progress this year. GPT-4.5 (Feb 2025) was a cautionary example — rumored much larger but "bad bang for the buck."

Inference scaling is one lever to get LLMs to solve extremely complex tasks on demand (DeepSeekMath-V2 achieved gold-level math via self-consistency + self-refinement; GPT Heavy Thinking / Pro are other examples).

Another major improvement came from training LLMs with tool use in mind. Hallucination rates keep improving, largely due to tool use. OpenAI's gpt-oss models were among the earlier open-weight models built with tool use in mind. Unfortunately, the open-source ecosystem hasn't fully caught up — many tools still default to non-tool-use mode, partly due to security ("would you trust a new intern to do this with this amount of access to your system?").

## 5. Word of the Year: Benchmaxxing

Benchmaxxing means there's a strong focus on pushing leaderboard numbers, sometimes to the point where benchmark performance becomes a goal in itself. Llama 4 scored extremely well across benchmarks, but users realized these scores didn't reflect real-world capabilities. "If the test set is public, it isn't a real test set." Benchmark numbers are no longer trustworthy indicators of LLM performance, though benchmarks remain necessary thresholds (below X = bad; above X ≠ better than another model above X).

## 6. AI for Coding, Writing, and Research

I see LLMs as tools that give people "superpowers." When used well, they make individuals substantially more productive.

**6.1 Coding.** Today, I still write most of the code I care about myself (where it matters that I understand the code and that it's correct), but I use LLMs to add the more mundane code around it. The trick is to recognize when and when not to use LLMs.

**6.2 Codebases.** I don't think code is or will become ephemeral or obsolete. Pure LLM-generated code bases don't replace expert-crafted code bases. An expert full-stack web developer will build a better platform than a random person prompting an LLM.

**6.3 Technical writing and research.** Writing a good technical book takes thousands of hours and deep familiarity. Rule of thumb: if a research article or book could have been generated by just prompting an LLM, then it's probably not novel and/or deep enough.

**6.4 LLMs and Burnout.** If the model does all the doing and the human mainly supervises, work can start to feel hollow. There is a special satisfaction in struggling with a hard problem and finally seeing it work. A good analogy is chess: chess engines surpassed human players decades ago, yet professional chess is still active and thriving. Used well, AI can accelerate learning — treat it as a partner rather than a replacement. But if AI is used to outsource thinking and coding entirely, it risks undermining motivation and long-term skill development.

## 7. The Edge: Private data

General capabilities will begin to plateau at some point (similar to GPT-4 to GPT-4.5) unless we keep inventing new training methods/architectures. To entrench LLMs in certain industries requires more domain specialization. LLM providers would love high-quality domain-specific data, but most companies approached have declined such deals precisely because the data is proprietary and core to their business differentiation (per multiple sources and a The Information article). Selling valuable proprietary data to OpenAI or Anthropic could be short-sighted.

LLM development is becoming increasingly commoditized — as LLM developers rotate between employers, bigger financial institutions, biotech companies, and others will develop competitive in-house LLMs on their private data. These don't have to be trained from scratch; open-weight models like DeepSeek V3.2, Kimi K2, and GLM 4.7 can be adapted and post-trained.

## 8. Building LLMs and Reasoning Models From Scratch

Last year, I decided to become independent and start my own company, mainly to have more time to work on my own research, books, Substack writing, and industry collaborations. As an independent researcher, consulting projects are part of what makes this setup sustainable. Over time, my goal is to reduce consulting and spend more time on long-form research and writing.

I am in the fortunate position that many companies have reached out about full-time roles, but for now, I plan to remain independent. Build A Large Language Model (From Scratch) has been translated into at least nine languages. I am currently working on a sequel, Build A Reasoning Model (From Scratch), which picks up from a pre-trained base model and explores inference-time scaling methods and reinforcement learning techniques aimed at improving reasoning. I'm currently halfway through chapter 6, which implements the reinforcement learning with verifiable rewards (GRPO) code.

## 9. Surprises in 2025 and Predictions for 2026

### 9.1 Noteworthy and Surprising Things in 2025

1. Several reasoning models already achieving gold-level math-competition performance (OpenAI unnamed model, Gemini Deep Think, open-weight DeepSeekMath-V2) — surprised it happened in 2025, not 2026.
2. Llama 4 (or Llama in general) fell almost completely out of favor; Qwen overtook Llama in popularity (per Nathan Lambert's ATOM project).
3. Mistral AI uses the DeepSeek V3 architecture for its latest flagship Mistral 3 model.
4. Many open-weight SOTA contenders emerged: Kimi, GLM, MiniMax, Yi.
5. Cheaper, efficient hybrid architectures becoming a bigger priority in leading labs (Qwen3-Next, Kimi Linear, Nemotron 3).
6. OpenAI released an open-weight model (gpt-oss).
7. MCP (joining the Linux Foundation) has already become the standard for tool and data access in agent-style LLM systems — faster than I expected.

### 9.2 Predictions for 2026

1. An industry-scale, consumer-facing diffusion model for cheap, reliable, low-latency inference, with Gemini Diffusion probably going first.
2. The open-weight community will slowly but steadily adopt LLMs with local tool use and increasingly agentic capabilities.
3. RLVR will more widely expand into other domains beyond math and coding (chemistry, biology, etc.).
4. Classical RAG will slowly fade as a default for document queries — replaced by better long-context handling and better "small" open-weight models.
5. A lot of LLM benchmark and performance progress will come from improved tooling and inference-time scaling rather than from training or the core model itself. The proportion of progress will come more from the inference than purely the training side this year.

Meta-lesson from 2025: progress in LLMs is less about a single breakthrough, and improvements are being made on multiple fronts via multiple independent levers (architecture tweaks, data quality, reasoning training, inference scaling, tool calling). Evaluation remains hard, benchmarks are imperfect, and good judgment about when and how to use these systems is still essential.

---
*Raw capture — immutable. Stripped of Substack nav/footer/comments/figure-URLs. Author: Sebastian Raschka (Raschka AI Research / RAIR Lab LLC), independent.*
