---
title: Research
layout: page
---

My academic profile including a CV, list of grants (projects) and bibliography can be found on my [ZHAW profile page](http://www.zhaw.ch/=stdm). A preserved version of my research at the University of Marburg can be found at my [Phillips University profile page](http://www.informatik.uni-marburg.de/~stadelmann/research.html).

## Statement of purpose

I am a **pattern recognition** researcher working on a wide variety of tasks on image, audio or generally "signal" data. I come from the tradition of the field of **artificial intelligence**, and my tool is **machine learning**. My research interest is to discover and understand how intelligent behaviour can be evoked through self-learning, including practical (robustness, generalization) and ethical (algorithmic bias) side effects. I focus on **deep learning** methodology, inspired by biological learning. Each task that I study has its own learning target (e.g., detection, classification, clustering, segmentation, novelty detection, control) and use case (e.g., predictive maintenance, multimedia indexing, document analysis, optical music recognition, industrial quality control, automated machine learning, automated game play), which in turn sheds light on different aspects of the learning process. 

## Recent work

### Robust and practical deep learning

Deep learning has reached the point of practical applicability in solving day-to-day tasks in many non-AI businesses, for instance manufacturing SMEs. Specific challenges arise and are tackled in our [applied research projects](http://stdm.github.io/downloads/papers/Beyond_ImageNet_preprint_2018.pdf), ranging from data quality and quantity issues to higher requirements on robustness and resilience of the models. For instance, segmenting newspaper pages into articles that semantically belong together is a necessary prerequisite for article-based information retrieval on print media collections like e.g. archives and libraries. It is challenging due to vastly differing layouts of papers, various content types and different languages, but commercially very relevant for e.g. media monitoring.

[<img alt="Examples of automatic segmentation" src="http://stdm.github.io/images/article_segmentation.jpg"/>](http://stdm.github.io/images/article_segmentation.jpg)

We have developed a [semantic segmentation approach](http://stdm.github.io/downloads/papers/ICDAR_2017.pdf) based on the visual appearance of each page. We apply a fully convolutional neural network (FCN) that we train in an end-to-end fashion to transform the input image into a segmentation mask in one pass. We show experimentally that the FCN performs very well: it outperforms a deep learning-based commercial solution by a large margin in terms of segmentation quality while in addition being computationally two orders of magnitude more efficient. The whole system is trained with only 5,500 images of which less than 500 are fully labeled.

[<img alt="Newspaper article segmentation architecture" src="http://stdm.github.io/images/fcnn_architecture.jpg"/>](http://stdm.github.io/images/fcnn_architecture.jpg)

Additionally, the existence of adversarial attacks on convolutional neural networks (CNN) questions the fitness of such models for serious applications. Such attacks manipulate an input image such that misclassification is evoked while still looking normal to a human observer - they are thus not easily detectable. In a different context, backpropagated activations
of CNN hidden layers - "feature responses" to a given input - have been helpful to visualize for a human "debugger" what the CNN "looks at" while computing its output. We have proposed a novel [detection method for adversarial examples](http://stdm.github.io/downloads/papers/ANNPR_2018c.pdf) to prevent attacks. We do so by tracking adversarial perturbations in feature responses, allowing for automatic detection using average local spatial entropy. The method does not alter the original network architecture and is fully human-interpretable. Experiments confirm the validity of our approach for state-of-the-art attacks
on large-scale models trained on ImageNet.

[<img alt="Detecting adversarial examples using local spatial entropy on feature response maps" src="http://stdm.github.io/images/adversarial_detection.jpg"/>](http://stdm.github.io/images/adversarial_detection.jpg)


### Learning to learn

[<img alt="Example clusterings" src="http://stdm.github.io/images/l2c_clustering.jpg"/>](http://stdm.github.io/images/l2c_clustering.jpg)

We have built a novel end-to-end neural network architecture that, once trained, directly outputs a probabilistic clustering of a batch of input examples in one pass. It estimates a distribution over the number of clusters and, for each number of clusters up to a maximum, distributions over the respective data partitioning. The neural network is trained in a
supervised fashion to group data by any perceptual similarity criterion based on pairwise labels (same/different group). It does not expect to have seen any of the groups that appear during model application already during training. We demonstrate promising performance on high-dimensional data like images (COIL-100) and speech (TIMIT). We call this [learning to cluster](http://stdm.github.io/downloads/papers/ANNPR_2018a.pdf).

[<img alt="Learning to cluster model architecture" src="http://stdm.github.io/images/l2c_architecture.jpg"/>](http://stdm.github.io/images/l2c_architecture.jpg)


### Optical music recognition (OMR)

[<img alt="Detection & recognition confidedences overlayed on a piece of handwritten music" src="http://stdm.github.io/images/MUSCIMA++.jpg"/>](http://stdm.github.io/images/MUSCIMA++.jpg)

Written music is a large and important part of cultural heritage worldwide. While there are many archives containing thousands of music scores, they are paper-based, so public access is cumbersome or even impossible. Digitization of these scores is currently impossible due to the non-availability of scanning software that can convert hand-written scores to machine-readable format (Optical Music Recognition – OMR). The DeepScore project aims at bringing bleeding edge technology form computer vision the field of OMR. The impact of OMR on how we curate, preserve and access music manuscripts cannot be overstated. Fully functional OMR would lead to a democratization of the musical cultural heritage by enabling cheap and efficient access by everyone. It would also enable more efficient music training, and enable orchestras to run cheaper and rehearse more efficiently. 

To facilitate deep learning for OMR, we built the [DeepScores](http://stdm.github.io/downloads/papers/ICPR_2018a.pdf) [dataset](https://tuggeluk.github.io/deepscores/) with the goal of advancing the state-of-the-art in small object recognition by placing the question of object recognition in the context of scene understanding. DeepScores contains high quality images of musical scores, partitioned into 300; 000 sheets of written music that contain symbols of different shapes and sizes. With close to a hundred million small objects, this makes our dataset not only unique, but also the largest public dataset. DeepScores comes with ground truth for object classification, detection and semantic segmentation. We provide baseline performances for object classification and intuition for the inherent difficulty that DeepScores poses to state-of-the-art object detectors like YOLO or R-CNN.

We introduced a novel object detection method, based on synthetic energy maps and the watershed transform, called [Deep Watershed Detector (DWD)](http://stdm.github.io/downloads/papers/ISMIR_2018.pdf). Our method is specifically tailored to deal with high resolution images that contain a large number of very small objects and is therefore able to process full pages of written music. We present state-of-the-art detection results of common music symbols and show DWD’s ability to work with synthetic scores equally well as on handwritten music.

[<img alt="Deep Watershed Detector architecture" src="http://stdm.github.io/images/dwd.jpg"/>](http://stdm.github.io/images/dwd.jpg)
 

### Voice recognition

[My PhD research](http://stdm.github.io/downloads/papers/PhdThesis_2010) focused on the task of speaker clustering: grouping speech segments by speaker identity without prior knowledge of the number or identity of speakers (a prerequisite for e.g. content-based media indexing). While speaker identification usually achieved accuracy percentages in their high nineties, the state of the art for the more complex task of clustering performed an order of magnitude worse. 

[<img alt="A clustering of 40 speakers from the TIMIT database" src="http://stdm.github.io/images/TIMIT_clustering.jpg"/>](http://stdm.github.io/images/TIMIT_clustering.jpg)

My 2009 ACM Multimedia paper on [Unfolding Speaker Clustering Potential – a Biomimetic Approach](http://stdm.github.io/downloads/papers/ACMMM_2009.pdf) (see also the [code](https://github.com/stdm/time_model)) not only analyzed this fact, but also identified deficiencies in modeling the sequence of speech features as the bottleneck responsible for the slump in performance. The prediction of potentially raising speaker clustering performance by an order of magnitude by better sequence modeling has led to exciting discoveries so far. We successively built deep learning models with more clustering capability to exploit the sequence information: a [simple CNN](http://stdm.github.io/downloads/papers/MLSP_2016.pdf), [CNN with optimized clustering loos](http://stdm.github.io/downloads/papers/MLSP_2017.pdf) and finally a [RNN](http://stdm.github.io/downloads/papers/ANNPR_2018b.pdf) to improve the capturing of prosodic voice information, to reduce the error rate for pure voice comparison by the predicted rate (see [code](https://github.com/stdm/ZHAW_deep_voice)). Additionally, using a [different clustering algorithm](http://stdm.github.io/downloads/papers/ICPR_2018b.pdf) on top of the simple CNN feature embeddings also proved valuable.

[<img alt="Architecture of the successful RNN model for speaker clustering" src="http://stdm.github.io/images/RNN_architecture.jpg"/>](http://stdm.github.io/images/RNN_architecture.jpg)


### Data science

I helped in creating one of Europe's first dedicated research centers for data science, the [ZHAW Datalab](http://www.zhaw.ch/datalab), and lead it since. Subsequently, my colleagues and I created one of Switzerland's first continuing education programs in data science, the [MAS Data Science](https://weiterbildung.zhaw.ch/de/school-of-engineering/programm/mas-data-science.html), where I teach machine learning. In 2015, we started rolling out the successful Datalab collaboration model country-wide in founding the [Swiss Alliance for Data-Intensive Services](https://www.data-service-alliance.ch/), a network of industrial and academic partner institutions that also furthered the [Swiss Conference on Data Science](https://sds2018.ch/) series of events that [started in Winterthur](https://www.zhaw.ch/en/research/inter-school-cooperation/datalab-the-zhaw-data-science-laboratory/sds2014/). The experience gained in these activities, together with the feedback from the applied research projects described above, lead to a [book](https://stdm.github.io/data-science-book/) I am co-editing together with my colleagues [Martin Braschler](www.zhaw.ch/=bram) and [Kurt Stockinger](www.zhaw.ch/=stog).


## Collaborations

I frequently collaborate with industry to work on exciting pattern recognition use cases. Partners from start-ups, SMEs and multi-national enterprises alike. 

In academia, I work together with the Machine Learning and Optimization Lab of [Martin Jaggi](https://mlo.epfl.ch/) at EPFL, [Marcello Pelillo](http://www.dsi.unive.it/~pelillo/) of the Ca'Foscari University of Venice, [Juergen Schmidhuber](http://people.idsia.ch/~juergen/)'s group at IDSIA, and [Friedhelm Schwenker](https://www.uni-ulm.de/in/neuroinformatik/mitarbeiter/f-schwenker/) of Ulm University, Insitute of Neural Information Processing. We have joint research projects and/or co-supervise PhD students.