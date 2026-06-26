# RAW — What comes next with reinforcement learning (Nathan Lambert, Interconnects)
Source: https://www.interconnects.ai/p/what-comes-next-with-reinforcement · 2025-06-09 · captured 2026-06-22 · channel: blog
- Lambert (coined RLVR in the Tülu 3 paper, fall 2024). Three avenues now that "RL works": (1) keep scaling RLVR for reasoning (more data/domains, no big algo breakthrough); (2) push RL to sparser domains (hours/days feedback — science, robotics); (3) continual learning.
- Key nuance: "scaling RL is the shortest path" means scaling techniques like current models, NOT unlocking complex new domains. "RL is not going to magically let us train models end-to-end that make entire codebases more efficient, run scientific experiments… There are major discoveries and infrastructure improvements needed."
- On Deep Research / Claude Code: trained with o1-style RL to get ROBUST at individual tasks; "the final long-horizon behavior is put together with prompting and letting the model run longer, not sparse credit assignment." (i.e. long-horizon = scaffold, not learned end-to-end.)
- Leans pessimist on sparse scaled RL (too similar to robotics where end-to-end RL is not SOTA). Longer RL runs → more frequent releases that feel like "continual learning."
- Strong opinion: true continual learning that learns from *you* is "a destiny to dystopia" — concentrates a powerful optimizer on intimate context. Prefers personalization / on-device / open "n-of-1" models.
Stake: researcher (AI2 at time of writing); open-models advocate; low commercial stake.
