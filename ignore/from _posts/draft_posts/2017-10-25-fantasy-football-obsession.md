---
layout: post
title: My Fantasy Football Obsession
tags: [fantasy football]
image: /psuanm5030.github.io/img/rescuetime_01.png
---

Earlier this summer, I decided that I was going to be prepared for my Fantasy Football draft this year.  No more last minute printouts and scrambling to listen to the latest podcasts.  For years, I have been under-prepared for my drafts, however, I still believe my mental model is sharp!  I tend to think I have a unique philosophy, a model (in my head) which considers more than just Yahoo/ESPNs latest rankings.  In the past few years, I have been working with the python and data sources such as [Yahoo Fantasy Sports API](https://developer.yahoo.com/fantasysports/guide/) and [nfldb](https://github.com/BurntSushi/nfldb/), and I finally felt like I had the time and, more importantly, the knowledge to employ my mental model in a structured and data-driven fashion.  This post outlines this fun project!

Overall

I started this effort envisioning something very basic, like a sorted listing of players with many different pieces of information stitched together.  In the end, I took my project a few steps further and ended up with a complete drafting tool.  Here is a listing of the elements involved in my drafting tool:

Acquisition of data via web scrapping (as well as flat file sources)
Aggregation of data at different levels of detail
Blending of information from various sources at a common level of detail
Feature generation and missing values imputation
Basic weighted model
Drafting tool
Visual insights tool
While those elements are part of the solution, many of them are at very low levels of implementation.  For example, the drafting tool was a new area for me and something that I would have loved to do so much more with.  I only scratched the surface there, as well as with my feature generation, model and automation of data acquisition.  There is much to do yet as well.  I haven't had the chance to review my model in-depth, let alone trying more sophisticated methods of fantasy success predication (which I "hear" arent much better than flipping a coin).

Check out my portfolio item, here, to see more.