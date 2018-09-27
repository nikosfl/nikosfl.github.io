---
title: Research
use-site-title: true
---

### Speaker Role Recognition
*and how to combine it with other speech processing tasks*  

Speaker role recognition is the task of assigning a specific role in a speaker-homogeneous segment, where a role is characterized by the task a speaker performs. Broadcast news programs, call centers, therapy sessions, or interviews are some examples of conversational scenarios where each participant performs some well-defined task and thus plays some role. 

The approaches that tackle this task depend on successful pre-processing steps applied on the conversation, such as speaker diarization or ASR. However, in real-world settings, this leads to error propagation. Additionally, knowledge of the roles can be proved useful for those pre-processing steps, as well. For example, the language used by an interviewer is expected to be different than the one used by the interviewee, and this is something which can be ideally exploited by a role-aware ASR system by using role-specific language models. 

What I am trying to do in this research thread is to combine speaker role recognition with other speech processing modules in order both to improve the performance of the role recognition itself and to provide useful information to the module it is combined with. In the paper "Role Annotated Speech Recognition for Conversational Interactions" (to be presented in SLT 2018) we are proposing an end-to-end system which does at the same time the jobs of an ASR, a diarization, and a role recognition module for the case of two speakers. In the paper "[Combined Speaker Clustering and Role Recognition in Conversational Speech](http://dx.doi.org/10.21437/Interspeech.2018-1654)" we are combining a speaker role recognizer with a traditional agglomerative speaker clustering module, leading to improved performance.

### Automating Behavioral Coding in Psychotherapy
*bring the machines in the game*  

Psychotherapy quality assessment is typically addressed by human raters who evaluate recorded sessions along specific behavioral codes, as defined by standard coding manuals. The recordings capture the complex series of interactions between the therapist and the client, and as such, they encode the active ingredients of the therapy. However, the time and cost barriers introduced by such a procedure lead to poor feasibility in real-world settings.

The question that naturally comes to mind - or, at least, to an engineer's mind - is "can we use machine learning techniques to facilitate this task?". This is exactly the question we are trying to answer through this research thread. With collaborators from the University of Washington, the University of Utah, the University of Pennsylvania, and the Arizona State University working in the clinical field, Signal Analysis and Interpretation Laboratory leads the engineering efforts towards automating behavioral coding in various types of psychotherapy, such as Motivational Interviewing (MI), Cognitive Behavioral Therapy (CBT), and CDC. Our paper "[Language Features for Automated Evaluation of Cognitive Behavior Psychotherapy Sessions](http://dx.doi.org/10.21437/Interspeech.2018-1518)" describes the first effort found in the literature for automated CBT evaluation. 
<!-- "[A technology prototype system for rating therapist empathy from audio recordings in addiction counseling](http://doi.org/10.7717/peerj-cs.59)" -->

A robust system for the task described depends heavily on a speech pipeline which, given the raw audio signal, 
* extracts the appropriate acoustic features, 
* detects the voiced regions (voice activity detection), 
* segments such regions into speaker-homogeneous segments (speaker change detection), 
* groups the resulted segments into same-speaker clusters (speaker clustering), 
* assigns each cluster either to the therapist or the client (speaker role recognition), 
* and converts the speech to text (automatic speech recognition)   
<!-- provide link with the kaldi pipeline -->

### Siamese CNNs for Speaker Change Detection
*a fancy way to compare similarities*  



### Automatic Sleep Staging Using HMMs
*or my 4 months in Czech Republic*  



### Acoustic Features for Robust Speech Recognition
*no, they are not MFCCs*  



### Identifying Saliency for Movie Summarization
*some movies are too boring to watch them from beginning to end, right?*  

If you are interested in the specific methodology and the results - and you know Greek - you can read my [report](/work/courses/movie_summary.pdf).
