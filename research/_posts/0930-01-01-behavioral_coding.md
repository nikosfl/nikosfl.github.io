---
layout: post
title: Automating Behavioral Coding in Psychotherapy
subtitle: bring the machines in the game
use-site-title: true
permalink: research/behavioral_coding
involved: 2017-2021
---

Psychotherapy quality assessment is typically addressed by human raters who evaluate recorded sessions along specific behavioral codes, as defined by standard coding manuals. 
The recordings capture the complex series of interactions between the therapist and the client, and as such, they encode the active ingredients of therapy. 
However, the time and cost barriers introduced by such a procedure lead to poor feasibility in real-world settings.

The question that naturally comes to mind - or, at least, to an engineer's mind - is "can we use machine learning techniques to facilitate this task?". This is exactly the question we are trying to answer through this research thread. With collaborators from the University of Washington, the University of Utah, the University of Pennsylvania, and the Arizona State University working in the clinical field, Signal Analysis and Interpretation Laboratory leads the engineering efforts towards automating behavioral coding in various types of psychotherapy, such as Motivational Interviewing (MI), Cognitive Behavioral Therapy (CBT), and coaching to decrease childhood obesity.
<!-- "[A technology prototype system for rating therapist empathy from audio recordings in addiction counseling](http://doi.org/10.7717/peerj-cs.59)" -->

<p align="center">
  <img src="/img/overview_pipeline.png" width="550">  
</p>
<em><font size="-1">
Automatic quality assessment of a psychotherapy session.  <br>
Image from <a href="http://dx.doi.org/10.3758/s13428-021-01623-4">Flemotomos et. al., Automated evaluation of psychotherapy skills using speech and language technologies, Behavior Research Methods, 2021</a>
</font></em>

A robust system for the task described depends heavily on a speech pipeline which, given the raw audio signal, 
* extracts the appropriate acoustic features, 
* detects the voiced regions (voice activity detection), 
* segments such regions into speaker-homogeneous segments ([speaker change detection](https://nikosfl.github.io/research/speaker_change_detection)), 
* groups the resulted segments into same-speaker clusters (speaker clustering), 
* assigns each cluster either to the therapist or the client ([speaker role recognition](https://nikosfl.github.io/research/srr)), 
* and converts the speech to text ([automatic speech recognition](https://nikosfl.github.io/research/asr_adaptation)).   

Such a pipeline is presented and analyzed in [this paper](https://rdcu.be/crPrw).

After the rich transcription of the dialogue between the therapist and the client is generated, natural language processing methods can be applied towards the final behavioral coding. [This paper](/work/papers/2018_IS_CBT_lang_features.pdf) describes the first effort found in the literature for automated CBT evaluation, purely based on linguistic features, while [here](/work/papers/2018_IS_multimodal_MISC.pdf) we introduce a multimodal system applied on MI data. Representations based on contextualized language models (e.g., BERT) can be applied to improve the predictive power of systems used in behavioral coding, as shown in our works [here](https://nikosfl.github.io/work/papers/2021_PLOS_CBT_BERT.pdf) -- where we introduce a multi-task model augmented with thepary-related metadata -- and [here](https://nikosfl.github.io/work/papers/2021_CBT_local_estimates.pdf) -- where we incorporate a local quality estimator to analyze long therapy sessions.   

<!-- last updated 2025-19-04 -->
