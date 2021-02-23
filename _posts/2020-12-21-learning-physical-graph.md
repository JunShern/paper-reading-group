---
layout: post
title: "Learning physical graph representations from visual scenes."
date: 2020-12-29 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vST0jP7TXaP_uHb2sXeqOOO7pGSZE4E8v10bitJJ-Is-iLXBh2eUiOWfATL750ra6NpAl1uynnNv2wt/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup002/"
reddit:
---

Bear, Daniel, et al. "Learning physical graph representations from visual scenes." Advances in Neural Information Processing Systems 33 (2020).

I was really excited to discover this paper recently. The question they tackle is one that's been on my mind for some time: "What form should a representation of scene understanding take to be suitable for physical reasoning tasks - with enough precision for manipulation and navigation, but also embedded with semantics, including contextual and abstract information?"

Their design is informed by human physical scene understanding, and the key properties of the proposed representation sound almost too good to be true: Graphs are spatially registered, follow semantically-meaningful hierarchical structure, capture abstract latent information at each node, have decoders that render corrigible scene reconstructions, and all this performed via self-supervised learning. On top of all that, we can perform symbolic manipulation of the scene? I know it's Christmas, but I wasn't expecting such a treat!

That said, the main drawback I can see is that the number of moving parts and custom modules in this architecture is immense. It is impressive that it all works together, but it sounds like a nightmare to implement and there seems to be a significant amount of human feature-engineering involved. Ablation experiments seem to justify each module, but I hope that down the road, we will be able to simplify this.

In the NeurIPS paper, they included a section on “Broader Impact” which I loved. Thoughtful words about their forward march towards intuitive physics, the focus on making representations interpretable, and even considerations about potential AI risks! It's clear that the authors have real vision and awareness about the place of their contribution in the field, and that this work was an earnest shot at a real, fundamental problem. I'm excited to see these representations put to good use in the near future!