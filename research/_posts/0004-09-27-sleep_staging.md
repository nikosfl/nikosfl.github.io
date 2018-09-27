---
layout: post
title: Automatic Sleep Staging Using HMMs
subtitle: or my 4 months in Czech Republic
use-site-title: true
permalink: research/sleep_staging
---

The aim of traineeship was to investigate the
use of Hidden Markov Models (HMMs) in automatic sleep staging from polysomnographic
(PSG) signals. HMMs have already been used in this field with promising results, but usually a
single HMM is being trained. Nikolaos Flemotomos developed unique algorithm for utilization
of “inner structure” of each single sleep stage by combination of more HMMs. The probability
of an observation given a particular state was computed according to a Gaussian Mixture Model
(GMM). An inseparable part of his work has also been working with other approaches like
signal segmentation, feature extraction, both in the frequency and in the time domain, and
feature selection by Principal Component Analysis (PCA). All implemented algorithms were
tested on real sleep PSG data, e.g. on the Sleep-EDF database, which consists of 61 PSG
recordings.

<!-- last updated: 2018-09-27 -->

