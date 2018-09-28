---
layout: post
title: Automating Behavioral Coding in Psychotherapy
subtitle: bring the machines in the game
use-site-title: true
permalink: research/behavioral_coding
involved: 2017-present
---

Psychotherapy quality assessment is typically addressed by human raters who evaluate recorded sessions along specific behavioral codes, as defined by standard coding manuals. The recordings capture the complex series of interactions between the therapist and the client, and as such, they encode the active ingredients of the therapy. However, the time and cost barriers introduced by such a procedure lead to poor feasibility in real-world settings.

The question that naturally comes to mind - or, at least, to an engineer's mind - is "can we use machine learning techniques to facilitate this task?". This is exactly the question we are trying to answer through this research thread. With collaborators from the University of Washington, the University of Utah, the University of Pennsylvania, and the Arizona State University working in the clinical field, Signal Analysis and Interpretation Laboratory leads the engineering efforts towards automating behavioral coding in various types of psychotherapy, such as Motivational Interviewing (MI), Cognitive Behavioral Therapy (CBT), and coaching to decrease childhood obesity.
<!-- "[A technology prototype system for rating therapist empathy from audio recordings in addiction counseling](http://doi.org/10.7717/peerj-cs.59)" -->

A robust system for the task described depends heavily on a speech pipeline which, given the raw audio signal, 
* extracts the appropriate acoustic features, 
* detects the voiced regions (voice activity detection), 
* segments such regions into speaker-homogeneous segments (speaker change detection), 
* groups the resulted segments into same-speaker clusters (speaker clustering), 
* assigns each cluster either to the therapist or the client ([speaker role recognition](https://nikosfl.github.io/research/srr)), 
* and converts the speech to text (automatic speech recognition).   
<!-- provide link with the kaldi pipeline -->

After the rich transcription of the dialogue between the therapist and the client, natural language processing methods can be applied towards the final behavioral coding. Our paper "[Language Features for Automated Evaluation of Cognitive Behavior Psychotherapy Sessions](http://dx.doi.org/10.21437/Interspeech.2018-1518)" describes the first effort found in the literature for automated CBT evaluation, purely based on linguistic features. In the paper "[Using Prosodic and Lexical Information for Learning Utterance-level Behaviors in Psychotherapy](http://dx.doi.org/10.21437/Interspeech.2018-2551)" we introduce a multimodal system applied on MI data.

<!-- last updated 2018-09-27 -->
