# RAW — Asymmetry of verification and verifier's rule (Jason Wei, jasonwei.net)
Source: https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law · 2025-07-15 · captured 2026-06-22 · channel: blog

## Thesis
Asymmetry of verification = the idea that some tasks are much easier to verify than to solve. "With reinforcement learning (RL) that finally works in a general sense, asymmetry of verification is becoming one of the most important ideas in AI."

## Understanding asymmetry through examples
- Sudoku / crosswords: slow to solve (try many candidates against constraints), trivial to check a given solution.
- Writing the code to operate a website like Instagram: takes a team of engineers many years; verifying whether the site works can be done quickly by a layperson.
- Solving BrowseComp problems: often requires browsing hundreds of websites, but verifying any given answer is much faster (you can directly search whether the answer meets the constraints).
- **Near-symmetry**: some tasks take a similar amount of time to verify as to solve — e.g. adding two 900-digit numbers; following someone else's data-processing code and verifying it works takes as long as writing it.
- **Inverse asymmetry (harder to verify than to propose)**: fact-checking all statements in an essay can take longer than writing it (Brandolini's law: "The amount of energy needed to refute bullshit is an order of magnitude bigger than that needed to produce it"). Many scientific hypotheses are harder to verify than to state — easy to state a novel diet ("Eat only bison and broccoli"), takes years to verify benefit.

## Improving asymmetry of verification
- Key realization: you can IMPROVE the asymmetry by front-loading research about the task.
- Competition math: trivial to check a proposed final answer if you have the answer key.
- Coding: tedious to read code and check correctness, but with test cases of ample coverage you can quickly check any solution (this is what Leetcode does).
- Sometimes you can improve but not trivialize: "Name a Dutch soccer player" — a list of famous Dutch players helps but verification still needs work.

## Verifier's rule (the central claim)
"If you consider the history of deep learning, we have seen that virtually anything that can be measured can be optimized. In RL terms, ability to verify solutions is equivalent to ability to create an RL environment."

> **Verifier's rule: The ease of training AI to solve a task is proportional to how verifiable the task is. All tasks that are possible to solve and easy to verify will be solved by AI.**

Five properties that govern trainability:
1. **Objective truth**: everyone agrees what good solutions are.
2. **Fast to verify**: any solution verifiable in a few seconds.
3. **Scalable to verify**: many solutions verifiable simultaneously.
4. **Low noise**: verification tightly correlated to solution quality.
5. **Continuous reward**: easy to rank goodness of many solutions for a single problem.

- Argues most popular AI benchmarks of the past decade fit #1–4; benchmarks that don't, don't become popular. Even where a solution is binary (failing #5), you get a continuous reward by averaging binary reward across many examples.
- Why verifiability matters most basically: "the amount of learning that occurs in neural networks is maximized when the above criteria are satisfied; you can take a lot of gradient steps where each step has a lot of signal. Speed of iteration is critical — it's the reason that progress in the digital world has been so much faster than progress in the physical world."

## AlphaEvolve as the exemplar
- "Perhaps the greatest public example of leveraging asymmetry of verification in the past few years is AlphaEvolve, developed by Google." Framed as "a very clever instantiation of guess-and-check that allows for ruthless optimization of an objective."
- Example problem: "Find the smallest outer hexagon that fits 11 unit hexagons" — fits all five properties.
- Note: AlphaEvolve-style problems can be seen as "overfitting" to a single problem — in scientific innovation you only care about solving the single unsolved (and valuable) problem: "train=test!"

## Relation to P = NP
- Both P=NP and verifier's rule concern asymmetry of verification, but verifier's rule makes NO claim about how long it takes AI to solve — in many cases it takes far more compute to solve than to verify given the answer key.
- Verifier's rule is BROADER than P=NP: it also applies to non-computational tasks (best catalyst to speed a reaction; best aerodynamic car design for fastest quarter-mile), provided we design systems to measure them quickly and at scale.

## Implications
- "It's exciting to consider a world where anything we can measure will be solved. We will likely have a jagged edge of intelligence, where AI is much smarter at verifiable tasks because it's so much easier to solve verifiable tasks."
- Recommends Alperen Keles's "Verifiability is the limit" post as related reading.
