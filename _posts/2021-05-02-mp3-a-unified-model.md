---
layout: post
title: "MP3: A Unified Model to Map, Perceive, Predict and Plan."
date: 2021-05-02 23:00:00 +0800
slides: "https://docs.google.com/presentation/d/e/2PACX-1vSzao-A2_U6s0hxKRe8NgZPH4fgXmmmHzvM2oR-9RtcHWy2BCNB6GTYGFztW4BYOZKvj3XrAWgTIoaZ/"
insta: "https://www.instagram.com/explore/tags/paperreadinggroup018/"
reddit: ""
twitter: ""
---

<a href="https://arxiv.org/pdf/2101.06806.pdf" target="_blank">
Casas, Sergio, Abbas Sadat, and Raquel Urtasun. "MP3: A Unified Model to Map, Perceive, Predict and Plan." arXiv preprint arXiv:2101.06806 (2021).
</a>

Two weeks ago, I virtually attended Nvidia GTC 2021 and made it a point to watch Raquel Urtasun's talk titled "A Future with Self-Driving Vehicles", knowing that her team at Uber (now Aurora) ATG consistently puts out outstanding autonomous driving research. Her excellent presentation focused on simulation, but also led me to this other new publication from the group.

Most autonomous vehicles today are built as a sequence of modules: Localization modules figure out where the vehicle is in mapped space, perception modules detect discrete object classes, prediction modules predict how those classes will move, planner modules plan a safe route around the environment, and control modules generate low-level steering and throttle actions.

A lot of effort thus goes into fine-tuning the performance of individual modules, but the overall system remains brittle because errors in upstream modules compound into downstream tasks, commonly useful information does not get shared between modules, and even the information that is shared tends to be funneled into lossy representations before passing it to the next module.

Therefore, I was glad to see this paper bravely take a step back and propose a different way of structuring the system. Some interesting ideas I liked: 
- The design is relatively lean, and all the pieces feed directly into enabling the planner. Going more end-to-end feels like a step in the right direction.
- Perception of dynamic objects is handled as an occupancy flow, which is more general and flexible than instance-based tracking.
- The currency of information transfer between the Backbone Network and the Scene Representation Networks are embeddings. Let's get rid of lossy representations!
- An urban driving planner may forever need to reason in interpretable representations, because that is the only way we only know how to enforce road rules (?).