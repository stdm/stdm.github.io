---
title: Research
layout: page
---

My academic profile including a CV, list of grants (projects) and bibliography can be found on my [ZHAW profile page](http://www.zhaw.ch/=stdm). An out-dated version of my research at University of Marburg can be found at my [Phillips University profile page](http://www.informatik.uni-marburg.de/~stadelmann/research.html).

## Statement of purpose

I am a **machine learning** researcher in the tradition of the field of **artificial intelligence**, focusing on **pattern recognition** problems. My research interest is to understand how learning works in general, especially the important properties of robustness (resilience) and generalization of methods. I focus on **deep learning** methodology to be inspired by biological learning. I fall back to a wide variety of pattern recognition problems to study these properties: each task has its own learning target (e.g., classification, clustering, segmentation, novelty detection, or control) and uses different architectures, which in turn shed light on different aspects of the learning process. 

## Recent work

Current work includes (see e.g. this [preprint](https://stdm.github.io/downloads/papers/Beyond_ImageNet_preprint_2018.pdf) and other recent papers):
  * I study the properties of recurrent **neural networks as universal controllers** (together with a PhD student co-supervised by Prof. Schmidhuber of IDSIA). The use case here is a meta-learning system for industrial image processing.
  * I analyze the **robustness of convolutional neural networks** to data quality and data quantity issues (together with a PhD student co-supervised at the Neuroinformatics Institute at the University of Ulm). The use case is vision-based quality control.
  * I explore the **connection between deep (generative) neural networks and game theory** (together with a PhD student co-supervised by Prof. Pelillo at the Ca’Foscari University of Venice). Use cases come from the computer vision community.
  * I keep extending my work on **speaker clustering** (see my [github repo](https://github.com/stdm/ZHAW_deep_voice) and [this paper](https://www.zhaw.ch/no_cache/de/forschung/personen-publikationen-projekte/detailansicht-publikation/publikation/212963/) for recent work) towards a fully neural end-to-end approach. The goal is to make the unsupervised clustering task able to learn from examples as of which cues in the data to use to form meaningful clusters. The use case is media indexing.
  * Besides classification and clustering tasks, I study **semantic segmentation** to learn about the ability of deep learning approaches on simultaneous multi-goal optimization. Use cases revolve around document recognition (optical music recognition; [print media segmentation](https://www.zhaw.ch/no_cache/de/forschung/personen-publikationen-projekte/detailansicht-publikation/publikation/212962/)) on data with considerably larger size and more objects of much smaller scale than in current benchmark data sets.
  * In the area of unsupervised learning, I study the properties of deep autoencoders. Use cases come from industrial predictive maintenance.

Current research interests go into the direction of deep reinforcement learning e.g. for home automation use cases as well as general meta learning and game playing.

## Success story

My PhD research focused on the task of speaker clustering: grouping speech segments by speaker identity without prior knowledge of the number or identity of speakers (a prerequisite for e.g. content-based media indexing). While speaker identification usually achieved accuracy percentages in their high nineties, the state of the art for the more complex task of clustering performed an order of magnitude worse. 

My 2009 ACM Multimedia paper on [Unfolding Speaker Clustering Potential – a Biomimetic Approach](http://www.informatik.uni-marburg.de/~stadelmann/download/papers/ACMMM_2009.pdf) (see also the [code](https://github.com/stdm/time_model)) not only analyzed this fact, but also identified deficiencies in modeling the sequence of speech features as the bottleneck responsible for the slump in performance. The prediction of potentially raising speaker clustering performance by an order of magnitude by better sequence modeling still impacts my work: Together with students and coworkers I explored possible advances in sequence learning and in the course was able to publish several papers on machine learning for signal processing: We already reduced the original error rate by >75% (see [Lukic et al., 2017](https://www.zhaw.ch/no_cache/de/forschung/personen-publikationen-projekte/detailansicht-publikation/publikation/212963/)).

This line of research also led me to introduce deep learning as a strategic research focus at ZHAW that is currently followed by several colleagues in different groups. From 2013-2017, I thus acquired 5.4 M CHF of 3rd party funding.
