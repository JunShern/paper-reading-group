---
layout: post
title: "Feature visualization."
date: 2021-03-06 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vQWs6gAovya6Z4_h6OETix0XKw_h4gDuzoHoGDUacqW2KEcZSdOAIa1OGhT_t7swxQ3z-2LGNIVJ30s/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup012/"
reddit: "https://www.reddit.com/r/MachineLearning/comments/lyude9/d_paper_reading_group_012_feature_visualization/"
twitter: "https://twitter.com/PaperReadingGrp/status/1368059328238743555"
---

Olah, Chris, Alexander Mordvintsev, and Ludwig Schubert. "Feature visualization." Distill 2.11 (2017): e7.

[Quick aside: This article is published on Distill, an online journal platform. Compared to standard journals where LaTeX PDFs reign supreme, all of the publications on this platform are built for the modern web, with all that browser technologies have to offer. If you haven't checked it out yet, head over to Distill.pub! I also urge interested readers to check out the original article to enjoy the full glory of their many interactive visualizations.]

This week's read has been around for a couple of years now, and I've often seen these psychedelic visualizations in passing, so I'm really happy to finally dig into some of the details. Having read this, I have to say that this is really creative out-of-the-box thinking, flipping the optimization variable and target in order to turn standard network optimization techniques into a microscope! 

It is also interesting to contrast this "discovery" style of research to the more common "invention" lines of work, where we are usually interested in obtaining some behaviour rather than free-form exploration. This style of exploration is more akin to early work in the natural sciences, where we dissect and observe in order to gleam understanding, often as a prerequisite before we can build new capabilities through engineering. Of course, both styles are important and not mutually exclusive.

Thinking about all this also leaves me with many follow-up questions. Given that we now have this working for images, can we also do the same thing for other modalities e.g. text or audio? And how far has this line of exploration progressed since 2017? I know that many sequel works are already published on Distill: For example, the authors have recently also put out a thread of articles on "Circuits" which explores emergent patterns of behaviour in groups of neurons common to different neural networks. So many papers, so little time!