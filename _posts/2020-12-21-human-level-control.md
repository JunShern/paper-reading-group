---
layout: post
title: "Human-level control through deep reinforcement learning."
date: 2020-12-21 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vTSdVB2OeK00y-t_Iz3mR5kw4qZBk_ol8E09CZilUSVYEZXWg1i0oeOxRUMMmHrhk1Ida5ZFXxq_Buz/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup001/"
reddit:
twitter: "https://twitter.com/PaperReadingGrp/status/1365669651867336709"
---

Mnih, Volodymyr, et al. "Human-level control through deep reinforcement learning." nature 518.7540 (2015): 529-533.

Published in 2015, this paper from DeepMind was really a landmark achievement (their first of many) demonstrating the real potential of deep reinforcement learning. RL is an old field which had primarily been of interest to Planning folk - but this paper managed to connect traditional RL techniques to neural networks, for an end-to-end trained agent which showed real promise for generalizable intelligence. This kicked off a frenzy of subsequent research and interest from the wider community, still sustained to this day.

Personally, this was the first RL paper I read, and it set a really high bar. The quality of the paper in terms of clarity, experiments, visualizations, and not least the results, is super inspiring to me. It's a great role model of research quality to aspire to. (This also happens to be the first Nature paper I have ever read; it is quite unusual for a CS paper to be published in Nature, but this paper does acknowledge its meaningful links to neuroscience which I enjoyed.)

One big theme of the paper is about achieving a “generalizable AI” which can play all these games. This hasn't exactly been achieved - yes, they use only one type of network with the same hyperparameters and initial conditions to solve all the games, but each game requires a new network instance trained from scratch. Seems to me like a meaningful next challenge would be to create a single instance of the agent which is able to play all the games well.

P.S. It was interesting to see that the paper has 3 primary and 16 additional authors! To me, this shows how collaborative DeepMind is, and also suggests that such groundbreaking and high-quality research really does take a village.