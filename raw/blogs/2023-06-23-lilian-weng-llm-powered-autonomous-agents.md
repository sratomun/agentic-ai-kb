# LLM Powered Autonomous Agents

Source: Lilian Weng, Lil'Log, June 23, 2023
URL: https://lilianweng.github.io/posts/2023-06-23-agent/
Captured: 2026-06-22 (full text via web_fetch)

> Cited as: Weng, Lilian. (Jun 2023). "LLM-powered Autonomous Agents". Lil'Log. https://lilianweng.github.io/posts/2023-06-23-agent/

---

Building agents with LLM as the core controller. Proof-of-concept demos cited: AutoGPT, GPT-Engineer, BabyAGI. "The potentiality of LLM extends beyond generating well-written copies, stories, essays and programs; it can be framed as a powerful general problem solver."

## Agent System Overview
LLM functions as the agent's brain, complemented by key components:
- **Planning** — (a) Subgoal and decomposition: break large tasks into smaller manageable subgoals. (b) Reflection and refinement: self-criticism and self-reflection over past actions, learn from mistakes.
- **Memory** — Short-term memory = in-context learning (restricted by finite context window). Long-term memory = external vector store with fast retrieval.
- **Tool use** — call external APIs for information missing from model weights.

## Component One: Planning

### Task Decomposition
- **Chain of thought (CoT)** (Wei et al. 2022): "think step by step"; uses more test-time computation to decompose hard tasks.
- **Tree of Thoughts** (Yao et al. 2023): extends CoT, explores multiple reasoning possibilities at each step, creating a tree; BFS or DFS search with each state evaluated by a classifier or majority vote.
- Decomposition done by (1) simple LLM prompting, (2) task-specific instructions, or (3) human inputs.
- **LLM+P** (Liu et al. 2023): outsource long-horizon planning to an external classical planner via PDDL (Planning Domain Definition Language). LLM translates problem to "Problem PDDL", classical planner generates plan, LLM translates back. Common in robotics setups, not many other domains.

### Self-Reflection
- **ReAct** (Yao et al. 2023): integrates reasoning and acting; action space = task-specific actions + language space. Template: Thought / Action / Observation (repeated). ReAct beats Act-only baseline on knowledge-intensive (HotpotQA, FEVER) and decision-making (AlfWorld, WebShop) tasks.
- **Reflexion** (Shinn & Labash 2023): dynamic memory + self-reflection; standard RL setup with binary reward; heuristic detects inefficient planning or hallucination (consecutive identical actions → same observation). Reflections added to working memory (up to three). Experiments on AlfWorld + HotpotQA; hallucination more common failure than inefficient planning in AlfWorld.
- **Chain of Hindsight (CoH)** (Liu et al. 2023): present sequence of past outputs annotated with feedback/ratings; SFT to predict best output. Adds regularization + randomly masks 0-5% of past tokens to avoid copying. Training data = WebGPT comparisons, summarization-from-human-feedback, hh-rlhf.
- **Algorithm Distillation (AD)** (Laskin et al. 2023): apply CoH idea to cross-episode RL trajectories; distill learning history into a neural net via behavioral cloning. Multi-episodic contexts of 2-4 episodes needed for near-optimal in-context RL. AD approaches RL^2 (upper bound) using only offline RL; learns faster than ED (expert distillation).

## Component Two: Memory
Human memory types mapped to agents:
- Sensory memory → learning embedding representations for raw inputs.
- Short-term / working memory (~7 items, 20-30s) → in-context learning (finite Transformer context window).
- Long-term memory → external vector store, fast retrieval.

### Maximum Inner Product Search (MIPS)
Save embeddings to vector store supporting fast MIPS; use approximate nearest neighbors (ANN) for speed. ANN algorithms reviewed: LSH (locality-sensitive hashing), ANNOY (random projection trees), HNSW (hierarchical navigable small world), FAISS (vector quantization / clustering), ScaNN (anisotropic vector quantization).

## Component Three: Tool Use
"Tool use is a remarkable and distinguishing characteristic of human beings."
- **MRKL** (Karpas et al. 2022): "Modular Reasoning, Knowledge and Language"; neuro-symbolic; LLM routes inquiries to expert modules (neural or symbolic). Experiment: harder to solve verbal math than explicit math; "knowing when and how to use the tools are crucial."
- **TALM** (Parisi et al. 2022) and **Toolformer** (Schick et al. 2023): fine-tune LM to use external tool APIs; dataset expanded if API call improves output quality.
- ChatGPT Plugins and OpenAI function calling — practical examples.
- **HuggingGPT** (Shen et al. 2023): ChatGPT as task planner selecting HuggingFace models. 4 stages: task planning, model selection, task execution, response generation. Challenges: efficiency, long context need, stability.
- **API-Bank** (Li et al. 2023): benchmark; 53 API tools, 264 dialogues, 568 API calls. Three eval levels: call the API, retrieve the API, plan API beyond retrieve-and-call.

## Case Studies
- **ChemCrow** (Bran et al. 2023): LLM + 13 expert chemistry tools (LangChain). Human experts judged ChemCrow > GPT-4 by a large margin even though LLM-based eval rated them equivalent → "potential problem with using LLM to evaluate its own performance on domains that requires deep expertise."
- **Boiko et al. (2023)**: LLM agents for scientific discovery; can browse, read docs, execute code, call robotics APIs. Risk test: 4/11 (36%) chemical-weapon requests were accepted; 7/11 rejected.
- **Generative Agents** (Park et al. 2023): 25 virtual characters in a sandbox (The Sims-inspired). Memory stream + retrieval (recency, importance, relevance) + reflection + planning/reacting. Emergent social behavior: information diffusion, relationship memory, coordination of social events.
- **AutoGPT, GPT-Engineer** proof-of-concepts. "A lot of code in AutoGPT is about format parsing." Full AutoGPT and GPT-Engineer system prompts reproduced in the post.

## Challenges (her own observations)
- **Finite context length**: limits historical information; vector stores less powerful than full attention.
- **Challenges in long-term planning and task decomposition**: "LLMs struggle to adjust plans when faced with unexpected errors, making them less robust compared to humans who learn from trial and error."
- **Reliability of natural language interface**: model outputs questionable — formatting errors, occasional "rebellious behavior" (refusing instructions). "Much of the agent demo code focuses on parsing model output."
