---
layout: post
title: "Concrete problems in AI safety."
date: 2021-01-09 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vRJE5pw-w5wa1C9zXNonAOMhnvt0bafzzov-XBXJsDrDmB9tNcnFLrj6-3ohZpLCaL_VDzDsfYqV5a9/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup004/"
reddit:
---

Amodei, Dario, et al. "Concrete problems in AI safety." arXiv preprint arXiv:1606.06565 (2016).

I've been reading a lot of books on AI safety recently. I finished some of the big ones including Superintelligence (Bostrom), Human Compatible (Russell), Life 3.0 (Tegmark). Each of these focuses on the long term existential risk of AI, which I do find compelling - but on the other hand, AI risks are already here today, out in the wild creating messes that nobody can understand or predict (Weapons of Math Destruction by O'Neil provides a good introduction to some aspects of this, as does the Netflix series The Social Dilemma).

This paper focuses on the latter problem of AI safety in current times ("In our opinion one need not invoke these extreme scenarios to productively discuss accidents, and in fact doing so can lead to unnecessarily speculative discussions that lack precision"). In any case, a lot of the problems listed here do overlap with the concerns for long-term AGI. My current instinct tells me that building a culture of safety around today's AI systems will also help us to navigate future risks better.

I encourage anybody in the boat as me to read the paper, which gives good concrete places to start. Note that while it is more of a survey paper which does not go deep into technicalities, good understanding of today's ML and RL systems are a prerequisite for sufficient context.

Noting some exciting research directions that stood out to me out of the ones mentioned in the paper:
- Reward as a multi-agent cooperation problem 
- Distant supervision 
- Incorporating uncertainty into neural networks 
- RL from expert demonstrations. 
- (Related to uncertainty?) Estimating performance on out-of-bound distributions.