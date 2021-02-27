---
layout: post
title: "World models."
date: 2021-01-02 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vRdVA9gpgC4S1qOopILgCYZ1vUnUgcg9-K3Un8pewFx4eW-nb2Z4QTH2ebPW0ZcN2KeIJskP0nnaLCs/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup003/"
reddit:
twitter: "https://twitter.com/PaperReadingGrp/status/1365670782236385283"
---

Ha, David, and Jürgen Schmidhuber. "World models." arXiv preprint arXiv:1803.10122 (2018).

This paper really knocked my socks off - the main mind-blow for me was the realization that when you use action priors to control the agent's dreams, you are literally walking in the mind of the agent and seeing the world through its own perspective. This feels like a really big idea, and definitely an interesting thread to pull on, in the direction of interpretability. "Walk a mile in someone's shoes to understand them" and all that.

Besides that, I really like this direction of decoupling the world model from the control model. The blue-sky vision would be to have generic "world model encoders" as the front-end for any environment, so that solving new problems would just be a question of figuring out the control model (which can be substantially simplified if the world model is given).

Digging further, I do have some reservations about their using generic image encodings as the main currency of state. Image reconstruction is not perfectly-aligned to the information actually needed for most tasks. The authors acknowledge this limitation as well: “Unsupervised learning cannot, by definition, know what will be useful for the task at hand … the tradeoff here is that we may not be able to reuse the VAE effectively for new tasks without retraining.” I'm thinking that the choice of representation will need to be adaptive based on the task - consider the different abstractions of perception needed to detect art forgery versus navigating a busy crosswalk - or wholly encapsulating, in which case the control model will have to on the work of deciding what information it needs.

There are also some bigger ideas in here about hierarchical learning by iteratively absorbing higher-level skills into the world model to reduce the cognitive load of the control model. This idea does resonate with me, and is worth thinking more about.