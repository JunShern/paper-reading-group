---
layout: post
title: "Causal effect inference with deep latent-variable models."
date: 2021-02-27 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vSlTCl3Bxds81LoDTZYB3hW5lfyGqc3R7Kxlj3NLcoIhESCPSXJDSpuU8MtVoOPCfdv777HA_LzSNrc/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup011/"
reddit:
twitter: "https://twitter.com/PaperReadingGrp/status/1365672573275570178"
---

Louizos, Christos, et al. "Causal effect inference with deep latent-variable models." arXiv preprint arXiv:1705.08821 (2017).

This week, I wanted to study a paper to give me a better grasp on the intersection of causality and machine learning, and how it appears in more traditional contexts (as compared to #ReadingGroup005!). This paper popped up several times in my literature search, and the publication history of the authors signal strong causal expertise, so I figured it would be a good a place to start.

I was pleased to find their introduction to the domain and the difficulties of confounding quite intuitive, and I love their approach of using NNs to automatically discover confounders (because despite issues with trusting NNs, I can still make peace with that more easily than trusting humans to pick out all the right confounders and proxies in every experiment). 

Funnily enough, I picked this paper so that I could study causality, but in the end I spent most of my time studying variational inference, trying to wrap my head around the VAE model.

Thinking about the wider direction of this work, I'll point out two limitations mentioned in the paper: "The proposed method does not currently deal with the related problem of selection bias" and "Problem assumes the causal model in Figure 1." CEVAE certainly promises to take a lot of the hairy work controlling confounders out of the process, but those two limitations still suggest the necessity of expert design. I wonder how far away we are from being able to blindly drop data into a causal algorithm and have it tell us the causal relationships of all the variables?