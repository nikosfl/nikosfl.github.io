---
layout: post
title: Siamese CNNs for Speaker Change Detection
subtitle: a fancy way to compare similarities
use-site-title: true
permalink: research/speaker_change_detection
---

Speaker change detection is the task of dividing a speech signal into speaker-homogeneous segments. In order to achieve this goal, the original signal is partitioned in consecutive small windows and we have to check how similar any two consecutive windows are. If they look similar enough, they are considered to belong to the same speaker. Otherwise, a speaker change point has been identified!

Following the definition of the problem, the research efforts in this field are focused on finding similarity metrics suitable for the particular task. Instead of trying to mathematically define such distance metrics, we can follow a data-driven approach and let a Deep Neural Network (DNN) architecture do the job. In this fun project, done as part of the requirements for the class "Deep Learning and its Applications", offered at USC in Fall 2017, I use siamese Convolutional Neural Nets (CNNs) experimenting with different system designs to tackle the problem. Siamese architectures have been introduced aiming exactly at learning a similarity metric between two inputs - originally applied on computer vision problems - and, as such, offer an ideal framework for the task of speaker change detection. You can find more information on the methods and the results visiting [my project page](http://nikosfl.github.io/sc-scd). 

<!-- last updated: 2018-09-27 -->
