# Scanner sources (vetted)

What the scanners pull from. Edit here to add/remove sources. `method`: `api` /
`web` (search or fetch) / `chrome` (logged-in or JS-gated).

## Focus filter (agents-centric)
Keep, in priority order: AI agents & agentic systems, agent frameworks/protocols
(MCP, tool use, orchestration), LLM reasoning & RL, evals/benchmarks for agents,
and exec-relevant industry moves (major model releases, funding, regulation,
notable product launches). Down-rank or drop: narrow theory with no applied
angle, unrelated ML (vision-only, bio, etc.) unless it clearly touches agents.

## arXiv — `api`
Endpoint: `https://export.arxiv.org/api/query` (follow the http→https redirect)
- Categories (core): cs.AI, cs.CL, cs.LG, cs.MA (multi-agent)
- Categories (added 2026-06-21): cs.SE (software-eng agents), cs.RO (robotics/
  embodied), cs.HC (human-agent interaction), cs.IR (retrieval/RAG/knowledge-graph/
  semantic-layer), cs.DB (text-to-SQL/data agents). Added to close a measured blind
  spot — agentic work in these categories was being under-sampled.
- Keywords (abstract): agentic, multi-agent, tool use, LLM agent, language agent,
  autonomous agent (plus: agent, function calling, reasoning, planning, RAG, MCP,
  orchestration for the weekly sweep)
- Lookback: last 7 days (weekly sweep) by submittedDate; full-year census on request
- Dedup key: arXiv id, version-stripped (e.g. 2406.12345)
- Note: `abs:` matches the abstract only, not full text. A paper is captured if ANY
  of its listed categories is in the set above (cross-listed papers count).

## News (events) — `web` + RSS  → news-scanner
*"What happened" — releases, funding, regulation, launches. Newsletters/roundups
live here, NOT in the blog scanner.*
- The Batch / DeepLearning.AI — https://www.deeplearning.ai/the-batch/ — newsletter
- TLDR AI — https://tldr.tech/ai — newsletter
- MIT Technology Review (AI) — https://www.technologyreview.com/topic/artificial-intelligence/ — web
- VentureBeat AI — https://venturebeat.com/category/ai/ — web
- Lab/company *announcement* posts (Anthropic, OpenAI, Google DeepMind, Meta AI) — web
- General web search for last-7-days agent news — web
- Dedup key: canonical URL

## Technical blogs (perspective) — `rss` / `web` / `chrome`  → blog-scanner
*"What it means / who thinks what" — durable technical essays, deep-dives,
post-mortems, and opinion from named authors and labs. NOT roundups/newsletters
(those are News, above). Discover each source's RSS/Atom feed at run time; fall back
to web_fetch; use Claude in Chrome only for JS/login-gated pages. Dedup by canonical
URL against `raw/blogs/` AND `raw/news/`.*

### Individual authors (the "who thinks what")
- Simon Willison — https://simonwillison.net/ (Atom: /atom/everything/)
- Andrej Karpathy — https://karpathy.github.io/ + gists/X
- Lilian Weng — https://lilianweng.github.io/
- Nathan Lambert — Interconnects — https://www.interconnects.ai/
- swyx / Latent Space (essays, not the podcast roundup) — https://www.latent.space/
- Sebastian Raschka — https://magazine.sebastianraschka.com/
- Eugene Yan — https://eugeneyan.com/
- Chip Huyen — https://huyenchip.com/blog/
- Hamel Husain — https://hamel.dev/
- Jason Wei — https://www.jasonwei.net/blog
- Ethan Mollick — One Useful Thing — https://www.oneusefulthing.org/
- Zvi Mowshowitz — Don't Worry About the Vase — https://thezvi.wordpress.com/
- Jack Clark — Import AI (essay sections) — https://importai.substack.com/
- Han Xiao (Jina) — https://jina.ai/news

### Labs & company engineering/research blogs
- Anthropic — https://www.anthropic.com/research + /engineering
- OpenAI — https://openai.com/news/research/
- Google DeepMind — https://deepmind.google/discover/blog/
- Meta AI (FAIR) — https://ai.meta.com/blog/
- Microsoft Research — https://www.microsoft.com/en-us/research/blog/
- Hugging Face — https://huggingface.co/blog
- LangChain — https://blog.langchain.dev/
- LlamaIndex — https://www.llamaindex.ai/blog
- Mistral — https://mistral.ai/news/
- Cognition (Devin) — https://cognition.ai/blog
- Sierra — https://sierra.ai/blog
- Together / Modal / Databricks — eng blogs (agents/infra)

### Market / strategy lens (VC firm blogs — fetchable)
- a16z — https://a16z.com/ (AI)
- Sequoia — https://www.sequoiacap.com/ (AI essays, e.g. Sonya Huang)
- Menlo Ventures — https://menlovc.com/perspective/

### Leaders & commentary (X / podcast / talk — opportunistic)
*Marquee figures whose *views* matter but who rarely write fetchable blogs. Capture
**opportunistically**: WebSearch to find the notable piece, then **Claude in Chrome**
to read the transcript (YouTube auto-captions, published podcast transcripts, X threads
as text). web_fetch first; Chrome only where it's gated/JS/transcript. Audio with NO
transcript page is out of scope — note and skip. `source_type:` = `interview` / `talk`
/ `post`. Lower capture rate than blogs — that's expected.*
**Tag the stake** on every commentary capture and person node (these voices often talk
their book): e.g. "GP at Sequoia — AI-fund book", "lab CEO — markets their model".
- **VCs:** Sonya Huang (Sequoia), Diana Hu (YC), Chamath Palihapitiya (Social Capital / All-In)
- **Scientists / lab leaders:** Geoffrey Hinton, Demis Hassabis (DeepMind), Jeff Dean (Google),
  Yann LeCun (Meta), Yoshua Bengio, Andrew Ng, Ilya Sutskever, Dario Amodei (Anthropic)
- _Person nodes are created on first capture (not pre-seeded); verify current
  affiliation via WebSearch before writing the node — titles change._

### Boundary note
A few sources are hybrids (Import AI, Latent Space): the **blog-scanner** pulls their
*technical essays/analysis*; the **news/briefing** layer handles their *roundups*.
The monthly cross-stack brief is a separate (newsletter) workflow — to be revisited.
