# RAW — Life lessons from reinforcement learning (Jason Wei, jasonwei.net)
Source: https://www.jasonwei.net/blog/life-lessons-from-reinforcement-learning · 2025-07-15 · captured 2026-06-22 · channel: blog

## Thesis
"Becoming an RL diehard in the past year and thinking about RL for most of my waking hours inadvertently taught me an important lesson about how to live my own life."

## On-policy as a life principle
- "One of the big concepts in RL is that you always want to be 'on-policy': instead of mimicking other people's successful trajectories, you should take your own actions and learn from the reward given by the environment."
- Imitation learning is useful to bootstrap to nonzero pass rate, but once you can take reasonable trajectories, "we generally avoid imitation learning because the best way to leverage the model's own strengths (which are different from humans) is to only learn from its own trajectories."
- Accepted instantiation: RL is a better way to train LMs to solve math word problems than supervised finetuning on human-written chains of thought.

## The life analogy
- We bootstrap via imitation learning (school) — reasonable. But Wei kept studying how others found success and imitating them. "Eventually I realized that I would never surpass the full ability of someone else because they were playing to their strengths which I didn't have."
- Examples: a researcher doing yolo runs more successfully because they built the codebase themselves; a soccer player keeping possession by leveraging strength he didn't have.
- "Beating the teacher requires walking your own path and taking risks and rewards from the environment."

## Wei's own strengths (playing on-policy)
Two things he enjoys more than the average researcher: (1) reading a lot of data, (2) doing ablations to understand the effect of individual components in a system.
- Once spent a few days reading data and giving each human annotator personalized feedback — the data turned out great and he gained insight into the task.
- "Earlier this year I spent a month going back and ablating each of the decisions that I previously yolo'ed while working on deep research." Sizable time, but he learned unique lessons about what type of RL works well, found it more fulfilling, and feels he's carving a stronger niche.

## Takeaway
"Imitation is good and you have to do it initially. But once you're bootstrapped enough, if you want to beat the teacher you must do on-policy RL and play to your own strengths and weaknesses."
