---
layout: post
title: Identifying Saliency for Movie Summarization
subtitle: let's create some trailers!
use-site-title: true
permalink: research/movie_summarization
involved: 2014
---

Humans have a unique capability of quickly identifying points of interests in a visual scene. Being able to efficiently extract, through a computational process, such salient segments in a video would lead to high-quality automated movie summaries. Motivated by neurobiological and psychophysical evidence about the way the human brain performs the specific task, we are interested in developing algorithms towards this direction.

My involvement in the particular field is due to a project that I undertook as part of the requirements for the class "Video and Image Analysis and Technology", offered at NTUA in Spring 2014, on movie summarization using attention and perception models. For this project, after implementing some of the techniques proposed in "[Multimodal Saliency and Fusion for Movie Summarization based on Aural, Visual and Textual Attention](http://dx.doi.org/10.1109/TMM.2013.2267205)", I conducted a series of original experiments.

Here is a 30% summary of the short film [The Most Beautiful Thing](https://www.youtube.com/watch?v=IP8psM4LWXk) using the algorithm I implemented

<video width="480" height="270" controls class="img-center">
  <source src="/work/classes/projects/tmbt_var_3.mp4" type="video/mp4">
  Your browser does not support embedded video.
</video>

and here is a 30% summary of the short film [Losses](https://www.youtube.com/watch?v=BMhXexbDmv8).

<video width="480" height="270" controls class="img-center">
  <source src="/work/classes/projects/los_var_3.mp4" type="video/mp4">
  Your browser does not support embedded video.
</video>

Note that the system implemented exploits only the visual stream of information, so you probably want to mute the videos to really understand the segments that the algorithm identified as salient.

If you are interested in the specific methodology, the theoretical background, and the comparative results - and you know Greek - you can read my [report](/work/classes/projects/eksaminiaia_video.pdf).

<!-- last updated: 2018-09-27 -->
