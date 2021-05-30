---
layout: post
title: "Emergent Prosociality in Multi-Agent Games Through Gifting."
date: 2021-05-30 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vToNnokdh-grQ3zNLKAPNlpkW3fc0m6Lp2V2QmazVPO9VFoJuBtYu_0X_uT6GBGIU7gMLtWFsWauHvc/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup019/"
reddit: "https://www.reddit.com/r/MachineLearning/comments/no6t7l/d_paper_reading_group_019_emergent_prosociality/"
twitter: "https://twitter.com/PaperReadingGrp/status/1398919401168986114"
---

<a href="https://arxiv.org/abs/2105.06593" target="_blank">
Wang, Woodrow Z., et al. "Emergent Prosociality in Multi-Agent Games Through Gifting." arXiv preprint arXiv:2105.06593 (2021).
</a>

Picked out this recent paper to learn more about multi-agent cooperation games. Working through a paper from an unfamiliar topic always teaches me a lot, and this time was no exception: The related work section is illuminating; I finally have a clearer picture of how ideas from reinforcement learning (the agents' policies, expected rewards) are connected to game theory; I also really liked the "basin of attraction" analysis and plot!

From the analysis, they were able to show that gifting actions do help with improving prosocial behavior, but it's still not clear to me why that happens. In the related work section, the paper notes that "Gifting allows agents to take a new action that may lower the risk their opponent experiences", but I did not manage to understand this connection.

I find it very important that the gifting approach relaxes the heavy-handed "reward-shaping" techniques that other coordination strategies rely on. This allows for a softer mechanism that can be enabled via environment design, whereas reward-shaping requires a God-like power to reshape agents' desires - which is only applicable in cases where you create the agents yourself.

Questions for me to follow up on (beyond the scope of this paper):
- Game theory seems to have a heavy focus on two-player games. How does it extend to N-players? Especially to large N, like country-sized populations. (This work does cover 3 and 4-player Stag Hunt, but in a naive way where each player plays N-1 two-player games with every other player. It doesn't seem like that would capture the full complexity of a multiplayer game.)
- How might these ideas transfer/apply to populations in the real world? In particular, I am interested to understand how big a gap there is between the simulated "economic man" who acts rationally toward a clear reward, contrasted to humans with complex goals and often act irrationally.