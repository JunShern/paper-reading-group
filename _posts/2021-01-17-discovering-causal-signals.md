---
layout: post
title: "Discovering causal signals in images."
date: 2021-01-17 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vSuk20uVnUsqoYeuc3zrUU4Px3g6OcK_ZKuCDSgvpKdtnSXj3WiksfoLv9QszV4soourE80Pvo9jwUz/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup005/"
reddit:
twitter: "https://twitter.com/PaperReadingGrp/status/1365671184356925448"
---

Lopez-Paz, David, et al. "Discovering causal signals in images." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2017.

Prior to this, my experience so far with causality only included reading The Book of Why by Judea Pearl, which sparked my interest and led me to Discovering (geddit?) this paper. But it seems to me that this work is entirely orthogonal to Pearl's do-calculus. I don't have enough knowledge to make meaningful contrast between Pearl's model-based methods and the observational discovery ones here, but if it does work as this paper claims, this could be hugely important.

As a beginner looking at all this, I will note that it was a brain-twister - I struggled to accept quite a number of the assumptions and chains-of-logic employed in their analysis. In the first place, does the relationship between car and wheel really constitute meaningful causality? The domain of visual features is also quite a curious one to look for causal signals in, though I can see that it is attractive due to the ubiquity of image data. I did however really like their exposition on the discovery of causal footprints, that was very clever.

Overall, I do love the attempt to address such a big and fundamental questions, as well as the creativity of the authors to reach their conclusion. This paper was published in 2017 and based on its claims, should have put to bed the critics who say that statistics and machine learning never amount to anything beyond correlations. But does this actually end the debate? If not, why? In any case, it's time to ramp up the literature review!

(As a side observation, it's also nice to see how far we have come in computer vision that we can simply plug-and-play convolutional nets that extract features from images to reliably use in other tasks!)