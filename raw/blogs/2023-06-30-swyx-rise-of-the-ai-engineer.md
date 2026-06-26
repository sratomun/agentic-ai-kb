# The Rise of the AI Engineer

- Author: swyx (Shawn Wang) + Alessio Fanelli
- Outlet: Latent.Space
- URL: https://www.latent.space/p/ai-engineer
- Date: 2023-06-30
- Fetched: 2026-06-22

---

We are observing a once in a generation "shift right" of applied AI, fueled by the
emergent capabilities and open source/API availability of Foundation Models. A wide
range of AI tasks that used to take 5 years and a research team to accomplish in 2013,
now just require API docs and a spare afternoon in 2023.

Karpathy: "In numbers, there's probably going to be significantly more AI Engineers than
there are ML engineers / LLM engineers. One can be quite successful in this role without
ever training anything."

Challenges in successfully evaluating, applying and productizing AI:
- Models: from GPT-4 and Claude down to the smallest open source HuggingFace, LLaMA models
- Tools: from chaining/retrieval/vector tools like LangChain, LlamaIndex, Pinecone to the
  emerging field of autonomous agents like Auto-GPT and BabyAGI
- Research/Progress: the sheer volume of papers/models/techniques is exponentially
  increasing — keeping on top of it all is almost a full time job.

swyx: "I think it IS a full time job. I think software engineering will spawn a new
subdiscipline, specializing in applications of AI and wielding the emerging stack
effectively, just as SRE, devops engineer, data engineer and analytics engineer
emerged." The emerging (and least cringe) version: AI Engineer. "This will likely be
the highest-demand engineering job of the decade."

"When it comes to shipping AI products, you want engineers, not researchers."

## The AI vs ML Engineer Flippening
There are 10x as many ML Engineer jobs as AI Engineer jobs on Indeed, but the higher
growth rate of "AI" leads me to predict this ratio will invert in 5 years. "In the near
future, nobody will recommend starting in AI Engineering by reading Attention is All You
Need, just like you do not start driving by reading the schematics for the Ford Model T."

## Why AI Engineers are Emerging Now
- Foundation Models are "few shot learners" with in-context learning and zero-shot
  transfer — the people creating the models don't fully know what they are capable of.
  People who AREN'T LLM researchers can find/exploit capabilities by spending time.
- Big labs have cornered scarce research talent to deliver "AI Research as a Service"
  APIs. ~5000 LLM researchers in the world, but ~50m software engineers. Supply
  constraints dictate an "in-between" class of AI Engineers will rise to meet demand.
- GPU hoarding.
- Fire, ready, aim: a PM/SWE can prompt an LLM and build/validate a product idea before
  getting specific data to finetune. "It's Waterfall vs Agile, all over again. AI is Agile."
- Python + JavaScript: TAM expansion as tools cater to JS devs (LangChain.js, Vercel AI SDK).
- Generative AI vs Classifier ML: a starkly different persona best wields LLMs.

## 1+2=3: Software 2.0 to Software 3.0
Karpathy's Software 2.0 (machine-learned NNs) → now "the hottest new programming language
is English." 2023's biggest theme: re-establishing the role of human-written code to
orchestrate and supplant LLM power (LangChain, Voyager code generation/reuse). The
primary architectural divide: "software atop intelligence" vs "intelligent software"
(Code Core vs LLM Core applications).

## AI Engineer Summit
Announces the first independently run, builder-oriented AI conference: The AI Engineer
Summit (ai.engineer), co-founded with Ben Dunphy of Reactathon. Tracks: AI UX, AI
Devtools, AI Infra, AI Agents, LLM tools (Langchain, Vector DBs), Open Source Models.

"AI Engineers will tame and ride Shoggoth. Let's make this a thing."

(Acknowledges Alessio Fanelli, Sarah Guo & Pranav Reddy of Conviction, and Ben Dunphy
for reviewing/supporting.)
