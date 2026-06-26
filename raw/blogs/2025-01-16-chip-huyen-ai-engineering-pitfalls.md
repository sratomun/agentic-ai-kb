# RAW — Common pitfalls when building generative AI applications (Chip Huyen, huyenchip.com)
Source: https://huyenchip.com/2025/01/16/ai-engineering-pitfalls.html · 2025-01-16 · captured 2026-06-22 · channel: blog
Note: A field-notes companion to *AI Engineering* (2025), drawn "both from public case studies and from my personal experience."

## The six pitfalls
1. **Use generative AI when you don't need it.** "Not everything is a nail." Example: a team used an LLM to schedule household energy use (claimed 30% bill cut) — but a trivial greedy heuristic ("do laundry / charge car after 10pm") or linear programming would likely beat it cheaper + more reliably. Also: anomaly detection, call-volume prediction, malnutrition detection ("really not recommended"). Key line: "'We solve the problem' and 'We use generative AI' are two very different headlines, and unfortunately, so many people would rather have the latter."

2. **Confuse 'bad product' with 'bad AI'.** Teams dismiss gen AI after users hate it — but the issue is usually **product/UX, not AI**. "Because everyone uses the same models nowadays, the AI components … are similar, and the differentiation is product." Examples:
   - Meeting-summary app: users didn't care about summary length — they only wanted **action items specific to them**.
   - LinkedIn skill-fit chatbot: users wanted **helpful**, not just **correct**, responses ("You're a terrible fit" is correct but useless → give gap-closing tips).
   - Intuit tax bot: users hated typing / didn't know what to ask → adding **suggested clickable questions** reduced friction and flipped feedback positive. (Nhung Ho, VP AI at Intuit.)

3. **Start too complex.** Examples of over-engineering: (1) agentic framework when direct API calls work; (2) agonizing over a vector DB when term-based retrieval works; (3) finetuning when prompting works; (4) semantic caching. Early external tooling abstracts away critical details (hard to debug) and adds bugs (framework default-prompt typos; silent prompt updates change your app's behavior). "Eventually, abstractions are good. But … as we're still in the early days of AI engineering, best practices are still evolving, we should be more vigilant when adopting any abstraction." (Directly anti-premature-agent-framework.)

4. **Over-index on early success.** Demo ≠ product; the last mile is brutal.
   - **LinkedIn**: 1 month to hit 80% of target experience, **+4 months to surpass 95%**; each subsequent 1% was discouragingly hard (esp. hallucinations).
   - Ecommerce AI-sales-assistant startup: 0→80% took as long as 80→90%. Challenges: accuracy/latency tradeoff (more planning/self-correction = more nodes = higher latency); **tool calling — hard for agents to differentiate similar tools**; tonal system-prompt requests not perfectly obeyed; hard to capture intent; infinite query combos make unit tests hard.
   - UltraChat (Ding et al. 2023): "the journey from 0 to 60 is easy, whereas progressing from 60 to 100 becomes exceedingly challenging."
   - Plus production roadblocks: **reliability** (10% of one team's API calls timed out; model swaps change behavior), **compliance** (copyright, data access, privacy, training-data lineage), **safety** (abuse, offensive outputs).

5. **Forgo human evaluation.** Many teams use **AI-as-a-judge / LLM-as-a-judge** and drop human eval entirely. But AI judges aren't deterministic; quality depends on judge model + prompt + use case, and must itself be evaluated/iterated. Best teams pair automated eval with **daily human eval** of 30–1000 outputs, which (1) correlates human vs AI judgments (diverging scores → suspect the judge), (2) reveals how users actually use the app, (3) catches behavior shifts via current-events knowledge. Annotation guidelines matter (if a human can't follow them, neither can the model; reusable as finetuning data). "Staring at data for just 15 minutes usually gives me some insight that could save me hours." Cites Greg Brockman: "Manual inspection of data has probably the highest value-to-prestige ratio of any activity in machine learning."

6. **Crowdsource use cases.** Execs unsure of strategy crowdsource ideas company-wide ("We hire smart people. Let them tell us what to do.") → "a million text-to-SQL models, a million Slack bots, and a billion code plugins." Individuals bias toward their own day-to-day pain, not highest-ROI problems. Without a big-picture strategy, you fragment into low-impact apps and wrongly conclude "gen AI has no ROI."

Stake: Author of *AI Engineering* (O'Reilly, 2025); practitioner-educator advising teams. Vendor-neutral; the throughline is "product + evaluation discipline beats shiny tooling." Now building in robotics.
