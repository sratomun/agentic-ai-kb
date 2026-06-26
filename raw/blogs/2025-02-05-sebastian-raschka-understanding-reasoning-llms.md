# Understanding Reasoning LLMs
## Methods and Strategies for Building and Refining Reasoning Models

**Sebastian Raschka, PhD — Feb 5, 2025 — Ahead of AI**
Source: https://magazine.sebastianraschka.com/p/understanding-reasoning-llms

---

This article describes the four main approaches to building reasoning models, or how we can enhance LLMs with reasoning capabilities. I hope this provides valuable insights and helps you navigate the rapidly evolving literature and hype surrounding this topic.

In 2024, the LLM field saw increasing specialization. Beyond pre-training and fine-tuning, we witnessed the rise of specialized applications, from RAGs to code assistants. I expect this trend to accelerate in 2025, with an even greater emphasis on domain- and application-specific optimizations (i.e., "specializations").

The development of reasoning models is one of these specializations. This means we refine LLMs to excel at complex tasks that are best solved with intermediate steps, such as puzzles, advanced math, and coding challenges. However, this specialization does not replace other LLM applications. Because transforming an LLM into a reasoning model also introduces certain drawbacks, which I will discuss later.

To give you a brief glimpse of what's covered below, in this article, I will:

1. Explain the meaning of "reasoning model"
2. Discuss the advantages and disadvantages of reasoning models
3. Outline the methodology behind DeepSeek R1
4. Describe the four main approaches to building and improving reasoning models
5. Share thoughts on the LLM landscape following the DeepSeek V3 and R1 releases
6. Provide tips for developing reasoning models on a tight budget

## How do we define "reasoning model"?

In this article, I define "reasoning" as the process of answering questions that require complex, multi-step generation with intermediate steps. For example, factual question-answering like "What is the capital of France?" does not involve reasoning. In contrast, a question like "If a train is moving at 60 mph and travels for 3 hours, how far does it go?" requires some simple reasoning. For instance, it requires recognizing the relationship between distance, speed, and time before arriving at the answer.

Most modern LLMs are capable of basic reasoning. So, today, when we refer to reasoning models, we typically mean LLMs that excel at more complex reasoning tasks, such as solving puzzles, riddles, and mathematical proofs.

Additionally, most LLMs branded as reasoning models today include a "thought" or "thinking" process as part of their response. Intermediate steps in reasoning models can appear in two ways. First, they may be explicitly included in the response. Second, some reasoning LLMs, such as OpenAI's o1, run multiple iterations with intermediate steps that are not shown to the user.

## When should we use reasoning models?

Reasoning models are designed to be good at complex tasks such as solving puzzles, advanced math problems, and challenging coding tasks. However, they are not necessary for simpler tasks like summarization, translation, or knowledge-based question answering. In fact, using reasoning models for everything can be inefficient and expensive. For instance, reasoning models are typically more expensive to use, more verbose, and sometimes more prone to errors due to "overthinking." Also here the simple rule applies: Use the right tool (or type of LLM) for the task.

## A brief look at the DeepSeek training pipeline

Before discussing four main approaches, I want to briefly outline the DeepSeek R1 pipeline, as described in the DeepSeek R1 technical report. This report serves as both an interesting case study and a blueprint for developing reasoning LLMs.

Note that DeepSeek did not release a single R1 reasoning model but instead introduced three distinct variants: DeepSeek-R1-Zero, DeepSeek-R1, and DeepSeek-R1-Distill.

**(1) DeepSeek-R1-Zero:** This model is based on the 671B pre-trained DeepSeek-V3 base model released in December 2024. The research team trained it using reinforcement learning (RL) with two types of rewards. This approach is referred to as "cold start" training because it did not include a supervised fine-tuning (SFT) step, which is typically part of reinforcement learning with human feedback (RLHF).

**(2) DeepSeek-R1:** This is DeepSeek's flagship reasoning model, built upon DeepSeek-R1-Zero. The team further refined it with additional SFT stages and further RL training, improving upon the "cold-started" R1-Zero model.

**(3) DeepSeek-R1-Distill:** Using the SFT data generated in the previous steps, the DeepSeek team fine-tuned Qwen and Llama models to enhance their reasoning abilities. While not distillation in the traditional sense, this process involved training smaller models (Llama 8B and 70B, and Qwen 1.5B–30B) on outputs from the larger DeepSeek-R1 671B model.

## The 4 main ways to build and improve reasoning models

Note: The exact workings of o1 and o3 remain unknown outside of OpenAI. However, they are rumored to leverage a combination of both inference and training techniques.

### 1) Inference-time scaling

One way to improve an LLM's reasoning capabilities is inference-time scaling: increasing computational resources during inference to improve output quality. A straightforward approach is clever prompt engineering. A classic example is chain-of-thought (CoT) prompting, where phrases like "think step by step" are included in the input prompt.

Another approach is the use of voting and search strategies. One simple example is majority voting where we have the LLM generate multiple answers, and we select the correct answer by majority vote. Similarly, we can use beam search and other search algorithms.

The DeepSeek R1 technical report categorizes common inference-time scaling methods (such as Process Reward Model-based and Monte Carlo Tree Search-based approaches) under "unsuccessful attempts."

I suspect that OpenAI's o1 and o3 models use inference-time scaling, which would explain why they are relatively expensive compared to models like GPT-4o.

### 2) Pure reinforcement learning (RL)

One of my personal highlights from the DeepSeek R1 paper is their discovery that reasoning emerges as a behavior from pure reinforcement learning (RL).

DeepSeek-R1-Zero was trained exclusively with reinforcement learning without an initial SFT stage. This is why they refer to it as "pure" RL. For rewards, instead of using a reward model trained on human preferences, they employed two types of rewards: an accuracy reward and a format reward.

- The accuracy reward uses the LeetCode compiler to verify coding answers and a deterministic system to evaluate mathematical responses.
- The format reward relies on an LLM judge to ensure responses follow the expected format, such as placing reasoning steps inside `<think>` tags.

Surprisingly, this approach was enough for the LLM to develop basic reasoning skills. The researchers observed an "Aha!" moment, where the model began generating reasoning traces as part of its responses despite not being explicitly trained to do so. This confirms that it is possible to develop a reasoning model using pure RL, and the DeepSeek team was the first to demonstrate (or at least publish) this approach.

### 3) Supervised finetuning and reinforcement learning (SFT + RL)

DeepSeek-R1, DeepSeek's flagship reasoning model, serves as a blueprint for building reasoning models. This model improves upon DeepSeek-R1-Zero by incorporating additional SFT and RL.

The DeepSeek team used DeepSeek-R1-Zero to generate "cold-start" SFT data. Using this cold-start SFT data, DeepSeek then trained the model via instruction fine-tuning, followed by another reinforcement learning (RL) stage. This RL stage retained the same accuracy and format rewards, plus a consistency reward to prevent language mixing.

The RL stage was followed by another round of SFT data collection: 600K Chain-of-Thought (CoT) SFT examples, plus 200K knowledge-based SFT examples created using the DeepSeek-V3 base model. These 600K + 200K SFT samples were then used for instruction-finetuning DeepSeek-V3 base before a final round of RL. All in all, this is very similar to regular RLHF except that the SFT data contains (more) CoT examples, and the RL has verifiable rewards in addition to human preference-based rewards.

### 4) Pure supervised finetuning (SFT) and distillation

Here distillation refers to instruction fine-tuning smaller LLMs, such as Llama 8B and 70B and Qwen 2.5 models (0.5B to 32B), on an SFT dataset generated by larger LLMs (DeepSeek-V3 and an intermediate checkpoint of DeepSeek-R1). The SFT data used is the same dataset that was used to train DeepSeek-R1.

The distilled models are noticeably weaker than DeepSeek-R1, but they are surprisingly strong relative to DeepSeek-R1-Zero, despite being orders of magnitude smaller.

The DeepSeek team also tested whether emergent reasoning could appear in smaller models by applying the same pure RL approach directly to Qwen-32B. Interestingly, the results suggest that distillation is far more effective than pure RL for smaller models. This aligns with the idea that RL alone may not be sufficient to induce strong reasoning abilities in models of this scale, whereas SFT on high-quality reasoning data can be a more effective strategy when working with small models.

### Conclusion

1. Inference-time scaling requires no additional training but increases inference costs. Still, it remains a no-brainer for improving the performance of already strong models. I strongly suspect that o1 leverages inference-time scaling.
2. Pure RL is interesting for research purposes (reasoning as an emergent behavior). However, in practical model development, RL + SFT is the preferred approach as it leads to stronger reasoning models.
3. RL + SFT is the key approach for building high-performance reasoning models. DeepSeek-R1 is a nice blueprint.
4. Distillation is attractive for creating smaller, more efficient models. However, the limitation is that distillation does not drive innovation or produce the next generation of reasoning models. For instance, distillation always depends on an existing, stronger model to generate the SFT data.

One interesting aspect I expect to see next is to combine RL + SFT (approach 3) with inference-time scaling (approach 1). This is likely what OpenAI o1 is doing, except it's probably based on a weaker base model than DeepSeek-R1, which explains why DeepSeek-R1 performs so well while remaining relatively cheap at inference time.

## Thoughts about DeepSeek R1

In short, I think they are an awesome achievement. One of the most fascinating takeaways is how reasoning emerged as a behavior from pure RL. And it's impressive that DeepSeek has open-sourced their models under a permissive open-source MIT license, which has even fewer restrictions than Meta's Llama models.

**How does it compare to o1?** I'd say it's roughly in the same ballpark. However, DeepSeek-R1 is more efficient at inference time. This suggests that DeepSeek likely invested more heavily in the training process, while OpenAI may have relied more on inference-time scaling for o1. That said, it's difficult to compare directly because OpenAI has not disclosed much about o1.

**The cost of training DeepSeek-R1.** Some have mentioned a ~$6 million training cost, but they likely conflated DeepSeek-V3 and DeepSeek-R1. The $6 million estimate is based on an assumed $2 per GPU hour and the number of GPU hours required for the final training run of DeepSeek-V3. However, the DeepSeek team has never disclosed the exact GPU hours or development cost for R1, so any cost estimates remain pure speculation.

## Developing reasoning models on a limited budget

Developing a DeepSeek-R1-level reasoning model likely requires hundreds of thousands to millions of dollars. Fortunately, model distillation offers a more cost-effective alternative.

**Sky-T1** — a small team trained an open-weight 32B model using only 17K SFT samples. The total cost? Just $450. According to their benchmarks, Sky-T1 performs roughly on par with o1.

**TinyZero** — a 3B parameter model that replicates the DeepSeek-R1-Zero approach (costs less than $30 to train). Even at just 3B parameters, TinyZero exhibits some emergent self-verification abilities, which supports the idea that reasoning can emerge through pure RL, even in small models.

**Journey Learning** — from the "O1 Replication Journey" paper. Shortcut learning refers to the traditional approach where models are trained using only correct solution paths. Journey learning, on the other hand, also includes incorrect solution paths, allowing the model to learn from mistakes. By exposing the model to incorrect reasoning paths and their corrections, journey learning may reinforce self-correction abilities.

---
*Raw capture — immutable. Stripped of Substack nav/footer/comments/figure-URLs. Author: Sebastian Raschka (Raschka AI Research / RAIR Lab LLC), independent.*
