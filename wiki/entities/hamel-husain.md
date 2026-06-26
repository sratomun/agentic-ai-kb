---
type: entity
entity_type: person
aliases: [hamelsmu, HamelHusain]
tags: [agents, person, evaluation]
affiliation: "Independent ML engineer / consultant via Parlance Labs (parlance-labs.com); ex-GitHub (creator of nbdev, ghapi; early code-search LLM research used by OpenAI for code embeddings) and ex-Airbnb (AutoML). Co-teaches the paid Maven course 'AI Evals for Engineers & PMs' with Shreya Shankar (4,500+ students)."
stake: Independent consultant who SELLS the discipline he writes about — runs a paid evals course and ships an evals tooling plugin (evals-skills). His 'evals/error-analysis are the bottleneck, not frameworks' thesis is also his business. Weight his hands-on practice heavily (30-50+ client engagements); discount the implicit 'you need to learn this from me' framing.
url: https://hamel.dev/
created: 2026-06-22
updated: 2026-06-22
---

# Hamel Husain

*The radar's leading practitioner voice on **product evals** — the argument that what gates a working LLM/agent product is error analysis and validated measurement, not the choice of framework. "Always look at the data."*

## Who they are
A machine-learning engineer with 20+ years of experience (Airbnb AutoML, GitHub — where he created **nbdev**, **ghapi**, and the early code-search LLM research OpenAI later used for code embeddings). He now works independently through **Parlance Labs**, helping teams "debug, analyze, and measure their AI systems" — work he packages under the banner **"evals."** He co-teaches the most prominent paid evals course on Maven (**AI Evals for Engineers & PMs**, 4,500+ students from 500+ companies incl. OpenAI, Anthropic, Google) with academic eval researcher **Shreya Shankar**, and writes the field's most-cited practitioner essays on the topic at hamel.dev. His lens is the **data scientist / applied ML engineer** — empirical, skeptical of vibes, allergic to off-the-shelf metrics.

**Stake:** He is an independent consultant **selling the exact discipline he champions** — a paid course, consulting, and an OSS plugin (evals-skills (his OSS eval toolkit)) all built around error analysis and judge validation. So when he says "evals are the bottleneck, frameworks aren't," note that evals are also his product. The discount is mild, though: the position is backed by 30-50+ hands-on client engagements and co-authored with a published academic, and his technical prescriptions (validate the judge like a classifier, binary pass/fail, ground synthetic data) are concrete and checkable, not salesmanship.

## What they argue (recurring stances)
- **Error analysis is the highest-ROI activity in AI engineering — and the one everyone skips.** Read your own production traces, open-code what went wrong, axial-code into a failure taxonomy, count the modes. The dominant failure is almost never the one the team assumed. Everything else (writing evals, picking metrics) comes *after*. ([[2025-03-24-blog-husain-field-guide|Field Guide]], [[2026-01-15-blog-husain-evals-faq|Evals FAQ]], [[2026-03-26-blog-husain-revenge-data-scientist|Revenge of the Data Scientist]].)
- **Evals, not frameworks, are the bottleneck.** The teams that succeed "barely talk about tools at all." Tool choice is downstream of process; off-the-shelf metrics (helpfulness/coherence/hallucination scores, ROUGE/BLEU) are "generic enough to be useless." Drive toward application-specific failure modes. (Field Guide, [[2025-10-01-blog-husain-eval-tools|Selecting an Evals Tool]].)
- **Treat the LLM judge as a classifier you must validate.** Human gold labels, train/dev/test, hill-climb the judge prompt, hold out a test set, and report **precision/recall (TPR/TNR), not accuracy** — "if a failure mode occurs 5% of the time, accuracy hides the system's true performance." Re-validate for drift. Prefer **binary pass/fail** over Likert. (Evals FAQ, Revenge, [[2026-03-02-blog-husain-evals-skills|Evals Skills]].)
- **"Criteria drift" means you can't automate away human review.** Per Shreya Shankar et al. (arXiv:2404.12272): people don't know their grading criteria until they look at outputs, so an LLM that invents-and-applies a rubric in one shot is a trap. Domain experts must label. (Evals FAQ, Revenge.)
- **The agent harness is data science.** Autonomous coding agents run inside a harness of tests, specs, *and metrics/observability* — that metric layer is experimental design, model evaluation, and production ML. Agents make the eval skill MORE valuable, not less. (Revenge, Evals Skills — both anchored on OpenAI's harness-engineering result.)
- **Retrieval isn't dead.** "Stop saying RAG is dead" — million-token context doesn't fix the economics or the precision problem; the future of RAG is better retrieval (late interaction, reasoning retrievers, context-rot awareness), not bigger context windows. ([[2025-07-11-blog-husain-rag-not-dead|Stop Saying RAG Is Dead]], with Ben Clavié.)

**Evolution 2025 → 2026:** Through 2025 he's the **methodology teacher** — the Field Guide and Evals FAQ codify error-analysis + judge-validation as a discipline, and the tool/RAG/Inspect pieces apply it. By 2026 his lens turns to the **agent era**: the same evals skills, now framed as (a) *what coding agents need to be taught* (evals-skills (his OSS eval toolkit) plugin) and (b) *why data scientists are essential, not obsolete*, because the agent harness's metric layer is data-science work. The throughline never changes: **look at the data.**

## Relationships
- writes at: hamel.dev; consults via Parlance Labs; co-teaches the Maven evals course with Shreya Shankar
- ex-employers: GitHub (nbdev/ghapi/code-search), Airbnb (AutoML)
- load-bearing voice in [[agent-evaluation]] · [[llm-as-judge]]; weighs in on [[agentic-rag]] · [[coding-agents]] · [[harness-engineering|harness engineering]]
- ships evals-skills (his OSS eval toolkit) (OSS plugin); reviews Braintrust · LangSmith · Arize Phoenix · [[inspect-ai]] (eval tools)
- recurring collaborators: Shreya Shankar · Bryan Bischof · Ben Clavié
- adjacent practitioner voices: [[chip-huyen]] · Eugene Yan
- anchors the [[debate-evals-vs-frameworks]] debate (evals-over-frameworks side)

## Writings (agent-relevant, 2025–26)
Captured (deep) source notes are wikilinked; the rest are enumerated for coverage. Scope = 2025-01-01 → 2026-06-22.
- 2025-01-19 — Thoughts On A Month With Devin (answer.ai; co-authored) — skeptical hands-on review of the Devin coding agent — https://www.answer.ai/posts/2025-01-08-devin.html
- 2025-03-24 — [[2025-03-24-blog-husain-field-guide|A Field Guide to Rapidly Improving AI Products]] *(deep)*
- 2025-06-23 — [[2025-06-23-blog-husain-inspect-ai|Inspect AI, An OSS Python Library For LLM Evals]] *(deep)* — annotated JJ Allaire guest lecture; the eval framework used by Anthropic/DeepMind/Grok/UK AISI
- 2025-07-11 — [[2025-07-11-blog-husain-rag-not-dead|Stop Saying RAG Is Dead]] *(deep)* — with Ben Clavié; 7-part series on the future of retrieval
- 2025-10-01 — [[2025-10-01-blog-husain-eval-tools|Selecting The Right AI Evals Tool]] *(deep)* — LangSmith vs Braintrust vs Arize Phoenix on the same task
- 2026-01-15 — [[2026-01-15-blog-husain-evals-faq|LLM Evals: Everything You Need to Know (AI Evals FAQ)]] *(deep)* — with Shreya Shankar; the canonical evals methodology reference
- 2026-01-18 — Why I Stopped Using nbdev (dev-tooling / personal AI stack; tangential to agents) — https://hamel.dev/blog/posts/ai-stack/
- 2026-03-02 — [[2026-03-02-blog-husain-evals-skills|Evals Skills for Coding Agents]] *(deep)*
- 2026-03-26 — [[2026-03-26-blog-husain-revenge-data-scientist|The Revenge of the Data Scientist]] *(deep)* — PyAI Conf talk

## Cited by (posts)
<!-- Auto-maintainable: the source notes that capture this person's posts. -->
- [[2025-03-24-blog-husain-field-guide]]
- [[2025-06-23-blog-husain-inspect-ai]]
- [[2025-07-11-blog-husain-rag-not-dead]]
- [[2025-10-01-blog-husain-eval-tools]]
- [[2026-01-15-blog-husain-evals-faq]]
- [[2026-03-02-blog-husain-evals-skills]]
- [[2026-03-26-blog-husain-revenge-data-scientist]]
