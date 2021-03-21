---
layout: post
title: "Accurate uncertainties for deep learning using calibrated regression."
date: 2021-03-21 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vS7-Gvz0nZ-c9ClNM9Vy65FeyZfheGoFEd7C5ZSCWvBA1rrwwodQ1MWRvG1KgIEZJ438h_AaGy4dnhz/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup014/"
reddit: "https://www.reddit.com/r/MachineLearning/comments/m9vspt/d_paper_reading_group_014_accurate_uncertainties/"
twitter: "https://twitter.com/PaperReadingGrp/status/1373613504725315585"
---

Kuleshov, Volodymyr, Nathan Fenner, and Stefano Ermon. "Accurate uncertainties for deep learning using calibrated regression." International Conference on Machine Learning. PMLR, 2018.

In situations where errors are tolerable and you only care about performance on net, overall test error may be sufficient for peace of mind, but calibrated uncertainty will likely be important to you whenever you have a model deployed in an environment where mistakes are costly (e.g. when your system is out in the wild affecting people's lives).

Given that motivation, these ideas of Platt scaling and calibrated regression seem useful and simple enough to implement that it should be common practice, so I wonder why I haven't seen this hit the mainstream? Even better, it is architecture-agnostic so I can imagine a well-written library would be plug-and-play: Just drop it in at the end of your training pipeline!

Coming back to that point, the fact that the algorithm is architecture-agnostic does make it easy for anyone to use, but it also hints that the technique doesn't have any real insight into what the forecast model is doing. My doubt then comes from the intuition that if you want your network to tell you how confident it is, shouldn't that confidence need to be a function of the input data instead of only y?

Also, even if we are able to demonstrate well-calibrated behaviour in the evaluation sets, at the end of the day, the recalibration model is itself also a model, so I imagine there must be some out-of-distribution cases where the recalibration fails. For example, how well would these calibration algorithms hold up against adversarial attacks? Perhaps there is a need for emphasis on the "given sufficient data" clause of the algorithm's promise.

I'm interested to take this out for a test-drive - but I would definitely push a bit harder on the limits and caveats of the calibration algorithm before I put my trust in the hands of an AI that claims to be calibrated.