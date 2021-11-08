---
layout: post
title: Speaker Adaptation for Automatic Speech Recognition
subtitle: make our voice assistants understand us more accurately
use-site-title: true
permalink: research/asr_adaptation
involved: 2020-2021
---

Automatic Speech Recognition (ASR) is the process of automatically getting the textual information that the raw audio signal is carrying, thus essentially converting speech to text. With the technological advances of the last few years, and especially with the advent of deep learning, machines can achieve remarkable results for the task, especially under relatively clean conditions. Additionally, even though traditionally ASR relies on convoluted architectures involving several different modules and components,
nowadays end-to-end solutions are successfully employed.

<p align="center">
  <img src="/img/malte_helmhold_unsplash.jpg" width="600">  
</p>
<em><font size="-1">
Automatic speech recognition revolutionalizes human-computer interaction.  <br>
Photo by Malte Helmhold on Unsplash.
</font></em>

Despite all those advances, both in terms of performance and in terms of simplicity, there is definitely still room for improvement. One aspect which holds promise for improved ASR performance is speaker (or, more broadly, domain/environment) adaptation. In general, since ASR systems depend on the data they are trained on, their performance can degrade when the conditions of use substantially differ from the training conditions. By the term adaptation we refer to the process of adjusting an already trained model to fit new, probably unseen, evaluation conditions. Thus, adaptation tries to compensate for the potential mismatch between training and testing data. 

<!-- Even though there has been a considerable amount of research on the topic of speaker (or accent/domain) adaptation for traditional ASR systems yielding significant
performance improvements, this is still a relatively under-explored topic in the context of end-to-end ASR. Being able to successfully adapt the ASR mechanism behind Siri would have a tremendous impact on the user experience, since Apple users expect their smart assistant to recognize their speech fast and accurately within their specific environment and using their own voice and accent. -->
