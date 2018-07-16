---
title: Research
layout: page
comments: true
---

This page is dedicated to the research of me and my group. My academic profile including a CV, list of grants (projects) and bibliography can also be found on my [ZHAW profile page](http://www.zhaw.ch/=stdm). A preserved version of my research at the University of Marburg can be found at my [Phillips University profile page](http://www.informatik.uni-marburg.de/~stadelmann/research.html).

### TOC
1. [Statement of purpose](#purpose)
2. [Recent work](#recent)
3. [Collaborations](#collaborations)
4. [Publications](#publications)

[<img alt="Collaboration" src="http://stdm.github.io/images/thilo-lasse-rheinfall.jpg"/>](http://stdm.github.io/images/thilo-lasse-rheinfall.jpg)


<a name="purpose"></a>
## Statement of purpose

I am a **pattern recognition** researcher working on a wide variety of tasks on image, audio or generally "signal" data. I come from the tradition of the field of **artificial intelligence**, and my tool is **machine learning**. My research interest is to discover and understand how intelligent behaviour can be evoked through self-learning, including practical (robustness, generalization) and ethical (algorithmic bias) side effects. I focus on **deep learning** methodology, inspired by biological learning. Each task that I study has its own learning target (e.g., detection, classification, clustering, segmentation, novelty detection, control) and use case (e.g., **predictive maintenance**, **speaker diarization**  for multimedia indexing, **document analysis**, **optical music recognition**, **computer vision** for industrial quality control, **automated machine learning**, **deep reinforcement learning** for automated game play or building control), which in turn sheds light on different aspects of the learning process. 


<a name="recent"></a>
## Recent work

1. [Robust and practical deep learning](#robust)
2. [Learning to learn](#l2l)
3. [Optical music recognition (OMR)](#OMR)
4. [Voice recognition](#voice)
5. [Data science](#datascience)

<a name="robust"></a>
#### Robust and practical deep learning

Deep learning has reached the point of practical applicability in solving day-to-day tasks in many non-AI businesses, for instance manufacturing SMEs. Specific challenges arise and are tackled in our [applied research projects](http://stdm.github.io/downloads/papers/Beyond_ImageNet_preprint_2018.pdf), ranging from data quality and quantity issues to higher requirements on robustness and resilience of the models. For instance, segmenting newspaper pages into articles that semantically belong together is a necessary prerequisite for article-based information retrieval on print media collections like e.g. archives and libraries. It is challenging due to vastly differing layouts of papers, various content types and different languages, but commercially very relevant for e.g. media monitoring.

[<img alt="Examples of automatic segmentation" src="http://stdm.github.io/images/article_segmentation.jpg"/>](http://stdm.github.io/images/article_segmentation.jpg)

We have developed a [semantic segmentation approach](http://stdm.github.io/downloads/papers/ICDAR_2017.pdf) based on the visual appearance of each page. We apply a fully convolutional neural network (FCN) that we train in an end-to-end fashion to transform the input image into a segmentation mask in one pass. We show experimentally that the FCN performs very well: it outperforms a deep learning-based commercial solution by a large margin in terms of segmentation quality while in addition being computationally two orders of magnitude more efficient. The whole system is trained with only 5,500 images of which less than 500 are fully labeled.

[<img alt="Newspaper article segmentation architecture" src="http://stdm.github.io/images/fcnn_architecture.jpg"/>](http://stdm.github.io/images/fcnn_architecture.jpg)

Additionally, the existence of adversarial attacks on convolutional neural networks (CNN) questions the fitness of such models for serious applications. Such attacks manipulate an input image such that misclassification is evoked while still looking normal to a human observer - they are thus not easily detectable. In a different context, backpropagated activations
of CNN hidden layers - "feature responses" to a given input - have been helpful to visualize for a human "debugger" what the CNN "looks at" while computing its output. We have proposed a novel [detection method for adversarial examples](http://stdm.github.io/downloads/papers/ANNPR_2018c.pdf) to prevent attacks. We do so by tracking adversarial perturbations in feature responses, allowing for automatic detection using average local spatial entropy. The method does not alter the original network architecture and is fully human-interpretable. Experiments confirm the validity of our approach for state-of-the-art attacks
on large-scale models trained on ImageNet.

[<img alt="Detecting adversarial examples using local spatial entropy on feature response maps" src="http://stdm.github.io/images/adversarial_detection.jpg"/>](http://stdm.github.io/images/adversarial_detection.jpg)

&nbsp;

<a name="l2l"></a>
#### Learning to learn

[<img alt="Example clusterings" src="http://stdm.github.io/images/l2c_clustering.jpg"/>](http://stdm.github.io/images/l2c_clustering.jpg)

We have built a novel end-to-end neural network architecture that, once trained, directly outputs a probabilistic clustering of a batch of input examples in one pass. It estimates a distribution over the number of clusters and, for each number of clusters up to a maximum, distributions over the respective data partitioning. The neural network is trained in a
supervised fashion to group data by any perceptual similarity criterion based on pairwise labels (same/different group). It does not expect to have seen any of the groups that appear during model application already during training. We demonstrate promising performance on high-dimensional data like images (COIL-100) and speech (TIMIT). We call this [learning to cluster](http://stdm.github.io/downloads/papers/ANNPR_2018a.pdf).

[<img alt="Learning to cluster model architecture" src="http://stdm.github.io/images/l2c_architecture.jpg"/>](http://stdm.github.io/images/l2c_architecture.jpg)

&nbsp;

<a name="OMR"></a>
#### Optical music recognition (OMR)

[<img alt="Detection & recognition confidedences overlayed on a piece of handwritten music" src="http://stdm.github.io/images/MUSCIMA++.jpg"/>](http://stdm.github.io/images/MUSCIMA++.jpg)

Written music is a large and important part of cultural heritage worldwide. While there are many archives containing thousands of music scores, they are paper-based, so public access is cumbersome or even impossible. Digitization of these scores is currently impossible due to the non-availability of scanning software that can convert hand-written scores to machine-readable format (Optical Music Recognition – OMR). The DeepScore project aims at bringing bleeding edge technology form computer vision the field of OMR. The impact of OMR on how we curate, preserve and access music manuscripts cannot be overstated. Fully functional OMR would lead to a democratization of the musical cultural heritage by enabling cheap and efficient access by everyone. It would also enable more efficient music training, and enable orchestras to run cheaper and rehearse more efficiently. 

To facilitate deep learning for OMR, we built the [DeepScores](http://stdm.github.io/downloads/papers/ICPR_2018a.pdf) [dataset](https://tuggeluk.github.io/deepscores/) with the goal of advancing the state-of-the-art in small object recognition by placing the question of object recognition in the context of scene understanding. DeepScores contains high quality images of musical scores, partitioned into 300; 000 sheets of written music that contain symbols of different shapes and sizes. With close to a hundred million small objects, this makes our dataset not only unique, but also the largest public dataset. DeepScores comes with ground truth for object classification, detection and semantic segmentation. We provide baseline performances for object classification and intuition for the inherent difficulty that DeepScores poses to state-of-the-art object detectors like YOLO or R-CNN.

We introduced a novel object detection method, based on synthetic energy maps and the watershed transform, called [Deep Watershed Detector (DWD)](http://stdm.github.io/downloads/papers/ISMIR_2018.pdf). Our method is specifically tailored to deal with high resolution images that contain a large number of very small objects and is therefore able to process full pages of written music. We present state-of-the-art detection results of common music symbols and show DWD’s ability to work with synthetic scores equally well as on handwritten music.

[<img alt="Deep Watershed Detector architecture" src="http://stdm.github.io/images/dwd.jpg"/>](http://stdm.github.io/images/dwd.jpg)
 
&nbsp;

<a name="voice"></a>
#### Voice recognition

[My PhD research](http://stdm.github.io/downloads/papers/PhdThesis_2010) focused on the task of speaker clustering: grouping speech segments by speaker identity without prior knowledge of the number or identity of speakers (a prerequisite for e.g. content-based media indexing). While speaker identification usually achieved accuracy percentages in their high nineties, the state of the art for the more complex task of clustering performed an order of magnitude worse. 

[<img alt="A clustering of 40 speakers from the TIMIT database" src="http://stdm.github.io/images/TIMIT_clustering.jpg"/>](http://stdm.github.io/images/TIMIT_clustering.jpg)

My 2009 ACM Multimedia paper on [Unfolding Speaker Clustering Potential – a Biomimetic Approach](http://stdm.github.io/downloads/papers/ACMMM_2009.pdf) (see also the [code](https://github.com/stdm/time_model)) not only analyzed this fact, but also identified deficiencies in modeling the sequence of speech features as the bottleneck responsible for the slump in performance. The prediction of potentially raising speaker clustering performance by an order of magnitude by better sequence modeling has led to exciting discoveries so far. We successively built deep learning models with more clustering capability to exploit the sequence information: a [simple CNN](http://stdm.github.io/downloads/papers/MLSP_2016.pdf), [CNN with optimized clustering loos](http://stdm.github.io/downloads/papers/MLSP_2017.pdf) and finally a [RNN](http://stdm.github.io/downloads/papers/ANNPR_2018b.pdf) to improve the capturing of prosodic voice information, to reduce the error rate for pure voice comparison by the predicted rate (see [code](https://github.com/stdm/ZHAW_deep_voice)). Additionally, using a [different clustering algorithm](http://stdm.github.io/downloads/papers/ICPR_2018b.pdf) on top of the simple CNN feature embeddings also proved valuable.

[<img alt="Architecture of the successful RNN model for speaker clustering" src="http://stdm.github.io/images/RNN_architecture.jpg"/>](http://stdm.github.io/images/RNN_architecture.jpg)

&nbsp;

<a name="datascience"></a>
#### Data science

I helped in creating one of Europe's first dedicated research centers for data science, the [ZHAW Datalab](http://www.zhaw.ch/datalab), and lead it since. Subsequently, my colleagues and I created one of Switzerland's first continuing education programs in data science, the [MAS Data Science](https://weiterbildung.zhaw.ch/de/school-of-engineering/programm/mas-data-science.html), where I teach machine learning. In 2015, we started rolling out the successful Datalab collaboration model country-wide in founding the [Swiss Alliance for Data-Intensive Services](https://www.data-service-alliance.ch/), a network of industrial and academic partner institutions that also furthered the [Swiss Conference on Data Science](https://sds2018.ch/) series of events that [started in Winterthur](https://www.zhaw.ch/en/research/inter-school-cooperation/datalab-the-zhaw-data-science-laboratory/sds2014/). The experience gained in these activities, together with the feedback from the applied research projects described above, lead to a [book](https://stdm.github.io/data-science-book/) I am co-editing together with my colleagues [Martin Braschler](www.zhaw.ch/=bram) and [Kurt Stockinger](www.zhaw.ch/=stog).

[<img alt="The data science skill set map" src="http://stdm.github.io/images/skillset.jpg"/>](http://stdm.github.io/images/skillset.jpg)

&nbsp;

&nbsp;

<a name="collaborations"></a>
## Collaborations

I frequently collaborate with industry to work on exciting pattern recognition use cases. Partners from start-ups, SMEs and multi-national enterprises alike. 

In academia, I frequently work together with the **Machine Learning and Optimization Lab** of [Martin Jaggi](https://mlo.epfl.ch/) at **EPFL**, [Marcello Pelillo](http://www.dsi.unive.it/~pelillo/) of the **Ca'Foscari University of Venice**, [Juergen Schmidhuber](http://people.idsia.ch/~juergen/)'s group at **IDSIA**, and [Friedhelm Schwenker](https://www.uni-ulm.de/in/neuroinformatik/mitarbeiter/f-schwenker/) of **Ulm University, Insitute of Neural Information Processing**. We have joint research projects and/or co-supervise PhD students.

If you are intgerested in a collaboration, please [contact](http://www.zhaw.ch/=stdm) me.

&nbsp;

&nbsp;

<a name="publications"></a>
## Publications

Counters: 1 book, 2 invited papers, 1 journal paper, 9 book chapters, 20 conference papers, 8 workshop papers, 1 position paper, 1 tech report, 2 theses.

| Year | Tag | Type| Publication |
| --- | --- | --- | --- |
| to appear | data science | chapter | Kurt Stockinger, Martin Braschler, and Thilo Stadelmann. "Lessons Learned from Challenging Data Science Case Studies". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | chapter | Lukas Hollenstein, Lukas Lichtensteiger, Thilo Stadelmann, Mohammadreza Amirian, Lukas Budde, Jürg Meierhofer, Rudolf M. Füchslin, and Thomas Friedli. "Unsupervised Learning and Simulation for Complexity Management in Business Operations". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | robust deep learning | chapter | Thilo Stadelmann, Vasily Tolkachev, Beate Sick, Jan Stampfli, and Oliver Dürr. **"Beyond ImageNet - Deep Learning in Industrial Practice"**. In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | chapter | Jürg Meierhofer, Thilo Stadelmann, and Mark Cieliebak. "**Data Products**". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | chapter | Thilo Stadelmann, Kurt Stockinger, Gundula Heinatz-Bürki, and Martin Braschler. "Data Scientists". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | chapter | Martin Braschler, Thilo Stadelmann, and Kurt Stockinger. "Data Science". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | chapter | Thilo Stadelmann, Martin Braschler, and Kurt Stockinger. "Introduction". In: Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). ["Applied Data Science - Lessons Learned for the Data-Driven Business"](https://stdm.github.io/data-science-book/). Springer, 2018. To appear. |
| to appear | data science | **book** | Martin Braschler, Thilo Stadelmann, and Kurt Stockinger (Editors). [**"Applied Data Science - Lessons Learned for the Data-Driven Business"**](https://stdm.github.io/data-science-book/). **Springer**, 2018. To appear. |
| 2018 | optical music recognition | workshop paper | Ismail Elezi, Lukas Tuggener, Marcello Pelillo, and Thilo Stadelmann. ["DeepScores and Deep Watershed Detection: current state and open issues"](https://stdm.github.io/downloads/papers/WoRMS_2018.pdf). In: Proceedings of the 1st International Workshop on Reading Music Systems (**WoRMS'18**), Paris, France, September 20, 2018. |
| 2018 | robust deep learning | **invited paper** | Thilo Stadelmann, Mohammadreza Amirian, Ismail Arabaci, Marek Arnold, Gilbert François Duivesteijn, Ismail Elezi, Melanie Geiger, Stefan Lörwald, Benjamin Bruno Meier, Katharina Rombach, and Lukas Tuggener. [**"Deep Learning in the Wild"**](https://stdm.github.io/downloads/papers/ANNPR_2018d.pdf). In: Proceedings of the 8th IAPR TC 3 Workshop on Artificial Neural Networks for Pattern Recognition (**ANNPR'18**), Siena, Italy, September 19-21, 2018. |
| 2018 | robust deep learning | conf. paper | Mohammadreza Amirian, Friedhelm Schwenker, and Thilo Stadelmann. [**"Trace and Detect Adversarial Attacks on CNNs using Feature Response Maps"**](). In: Proceedings of the 8th IAPR TC 3 Workshop on Artificial Neural Networks for Pattern Recognition (**ANNPR'18**), Siena, Italy, September 19-21, 2018. |
| 2018 | voice recognition | conf. paper | Thilo Stadelmann, Sebastian Glinski-Haefeli, Patrick Gerber, and Oliver Dürr. ["Capturing Suprasegmental Features of a Voice with RNNs for Improved Speaker Clustering"](https://stdm.github.io/downloads/papers/ANNPR_2018b.pdf). In: Proceedings of the 8th IAPR TC 3 Workshop on Artificial Neural Networks for Pattern Recognition (**ANNPR'18**), Siena, Italy, September 19-21, 2018. |
| 2018 | learning to learn | conf. paper | Benjamin Bruno Meier, Ismail Elezi, Mohammadreza Amirian, Oliver Dürr, and Thilo Stadelmann. [**"Learning Neural Models for End-to-End Clustering"**](). In: Proceedings of the 8th IAPR TC 3 Workshop on Artificial Neural Networks for Pattern Recognition (**ANNPR'18**), Siena, Italy, September 19-21, 2018. |
| 2018 | optical music recognition | conf. paper | Lukas Tuggener, Ismail Elezi, Jürgen Schmidhuber, and Thilo Stadelmann. [**"Deep watershed detector for music object recognition"**](https://stdm.github.io/downloads/papers/ISMIR_2018.pdf). In: Proceedings of the 19th International Society for Music Information Retrieval Conference (**ISMIR'18**), Paris, 23. - 27. September 2018. Paris: Society for Music Information Retrieval. [DOI](https://doi.org/10.21256/zhaw-3760). |
| 2018 | voice recognition | conf. paper| Feliks Hibraj, Sebastiano Vascon, Thilo Stadelmann, and Marcello Pelillo. ["Speaker clustering using dominant sets"](https://stdm.github.io/downloads/papers/ICPR_2018b.pdf). In: Proceedings of the 24th International Conference on Pattern Recognition (ICPR 2018). 24th International Conference on Pattern Recognition (**ICPR'18**), Beijing, China, 20-28 August 2018. Beijing: IAPR. [DOI](https://doi.org/10.21256/zhaw-4254). |
| 2018 | optical music recognition | conf. paper| Lukas Tuggener, Ismail Elezi, Jürgen Schmidhuber, Marcello Pelillo, and Thilo Stadelmann. [**"DeepScores: a dataset for segmentation, detection and classification of tiny objects"**](https://stdm.github.io/downloads/papers/ICPR_2018a.pdf). In: Proceedings of the 24th International Conference on Pattern Recognition. 24th International Conference on Pattern Recognition (**ICPR'18**), Beijing, China, 20-28 August 2018. Beijing: IAPR. 1-6. [DOI](https://doi.org/10.21256/zhaw-4255). |
| 2017 | document recognition | conf. paper | Benjamin Meier, Thilo Stadelmann, Jan Stampfli, Marek Arnold, and Mark Cieliebak. ["**Fully convolutional neural networks for newspaper article segmentation**"](https://stdm.github.io/downloads/papers/ICDAR_2017.pdf). In: Proceedings of the 14th IAPR International Conference on Document Analysis and Recognition (**ICDAR'17**). 14th IAPR International Conference on Document Analysis and Recognition (ICDAR), Kyoto Japan, November 13-15, 2017. Kyoto, Japan: CPS. [DOI](https://doi.org/10.21256/zhaw-1533). |
| 2017 | voice recognition | conf. paper| Yanick X. Lukic, Carlo Vogt, Oliver Dürr, and Thilo Stadelmann. ["Learning Embeddings for Speaker Clustering Based on Voice Equality"](https://stdm.github.io/downloads/papers/MLSP_2017.pdf). In: Proceedings of the 27th IEEE International Workshop on Machine Learning for Signal Processing (**MLSP'17**). Roppongi, Tokyo, Japan: IEEE. [DOI](https://doi.org/10.21256/zhaw-3762). |
| 2016 | voice recognition| conf. paper| Yanick Lukic, Carlo Vogt, Oliver Dürr, and Thilo Stadelmann. ["**Speaker Identification and Clustering using Convolutional Neural Networks**"](https://stdm.github.io/downloads/papers/MLSP_2016.pdf). In: Proceedings of IEEE International Workshop on Machine Learning for Signal Processing (**MLSP'16**). Salerno: IEEE. [DOI](https://doi.org/10.21256/zhaw-3761). |
| 2016 | data science | chapter | Kurt Stockinger, Thilo Stadelmann, and Andreas Ruckstuhl. ["Data Scientist als Beruf"](https://stdm.github.io/downloads/papers/HMD_2016.pdf). Big Data – Grundlagen, Systeme und Nutzungspotenziale, Springer Verlag, **Edition HMD** 59-81, 2016. [DOI](https://doi.org/10.1007/978-3-658-11589-0_4). |
| 2015 | AI | **invited paper** | Jean-Daniel Dessimoz, Jana Koehler, and Thilo Stadelmann. [**"AI in Switzerland"**](https://stdm.github.io/downloads/papers/AIMAG_2015.pdf). **AI Magazine**. 36(2), S. 102-105, 2015. [DOI](https://doi.org/10.21256/zhaw-3642). |
| 2015 | data science | position paper | Thilo Stadelmann, Mark Cieliebak, and Kurt Stockinger. ["Toward automatic data curation for open data"](https://stdm.github.io/downloads/papers/ERCIM_2015.pdf). **ERCIM News**. 2015(100), S. 32-33. [DOI](https://doi.org/10.21256/zhaw-3643). |
| 2014 | data science | chapter | Kurt Stockinger, and Thilo Stadelmann. ["Data Science für Lehre, Forschung und Praxis"](https://stdm.github.io/downloads/papers/HMD_2014.pdf). **HMD Praxis der Wirtschaftsinformatik**. 51(4), S. 469-479, 2014. [DOI](https://doi.org/10.21256/zhaw-3759). |
| 2013 | data science | conf. paper | Thilo Stadelmann, Kurt Stockinger, Martin Braschler, Mark Cieliebak, Gerold Baudinot, Oliver Dürr, and Andreas Ruckstuhl. ["**Applied data science in Europe**: challenges for academia in keeping up with a highly demanded topic"](ECSS_2013.pdf). In: Proceedings of the 9th European Computer Science Summit (**ECSS'13**), Amsterdam, October 8–9, 2013. |
| 2012 | automatic driving | conf. paper | Thilo Stadelmann, Sven Johr, Michael Ditze, Florian Dittman, and Viktor Fässler. ["FABELHAFT - Fahrerablenkung: Entwicklung eines Meta-Fahrerassistenzsystems durch Echtzeit-Audioklassifikation"](https://stdm.github.io/downloads/papers/VDIFASIS_2012.pdf). In Proceedings of 28. **VDI-VW Gemeinschaftstagung Fahrerassistenzsysteme und Integrierte Sicherheit**, Wolfsburg, Germany, October 10.-11., 2012. VDI Wissensforum. |
| 2010 | voice recognition | PhD thesis | Thilo Stadelmann. ["**Voice Modeling Methods for Automatic Speaker Recognition**"](https://stdm.github.io/downloads/papers/PhdThesis_2010.pdf). Dissertation, Philipps-Universität Marburg. [Available online, 2010](http://archiv.ub.uni-marburg.de/diss/z2010/0465/view.html). |
| 2010 | voice recognition | tech report | Thilo Stadelmann & Bernd Freisleben. ["**On the MixMax Model and Cepstral Features for Noise-Robust Voice Recognition**"](https://stdm.github.io/downloads/papers/TR_2010.pdf). Technical report, Philipps-Universität Marburg, April 2010.
| 2010 | voice recognition | workshop paper | Christian Beecks, Thilo Stadelmann, Bernd Freisleben, and Thomas Seidl. ["Visual Speaker Model Exploration"](https://stdm.github.io/downloads/papers/ICME_2010.pdf), In Proceedings of the IEEE International Conference on Multimedia and Expo (**ICME'2010**), pages 727-728, Singapore, July 19-23, 2010, IEEE. |
| 2010 | robust machine learning | conf. paper | Thilo Stadelmann, Yinghui Wang, Matthew Smith, Ralph Ewerth, and Bernd Freisleben. ["**Rethinking Algorithm Development and Design in Speech Processing**"](https://stdm.github.io/downloads/papers/ICPR_2010b.pdf). In Proceedings of the 20th International Conference on Pattern Recognition (**ICPR'10**), pages 4476-4479, Istanbul, Turkey, August 2010a. IAPR. |
| 2010 | voice recognition | conf. paper | Thilo Stadelmann and Bernd Freisleben. ["Dimension-Decoupled Gaussian Mixture Model for **Short Utterance Speaker Recognition**"](https://stdm.github.io/downloads/papers/ICPR_2010a.pdf). In Proceedings of the 20th International Conference on Pattern Recognition (**ICPR'10**), pages 1602-1605, Istanbul, Turkey, August 2010a. IAPR. |
| 2009 | video analysis | workshop paper | Markus Mühling, Ralph Ewerth, Thilo Stadelmann, Bing Shi, and Bernd Freisleben. ["University of Marburg at TRECVID 2009: High-Level Feature Extraction"](https://stdm.github.io/downloads/papers/TRECVID_2009.pdf). In Proceedings of TREC Video Retrieval Evaluation Workshop (**TRECVid'09**). [Available online, 2009](http://www-nlpir.nist.gov/projects/tvpubs/tv.pubs.org.htm). |
| 2009 | SoA | workshop paper | Ernst Juhnke, Dominik Seiler, Thilo Stadelmann, Tim Dörnemann, and Bernd Freisleben. ["LCDL: An Extensible Framework for Wrapping Legacy Code"](https://stdm.github.io/downloads/papers/ERPAS_2009.pdf). In Proceedings of International Workshop on @WAS Emerging Research Projects, Applications and Services (**ERPAS'09**), pages 638-642, Kuala Lumpur, Malaysia, December 2009. |
| 2009 | SoA | conf. paper | Dominik Seiler, Ralph Ewerth, Steffen Heinzl, Thilo Stadelmann, Markus Mühling, Bernd Freisleben, and Manfred Grauer. ["Eine Service-Orientierte Grid-Infrastruktur zur Unterstützung Medienwissenschaftlicher Filmanalyse"](https://stdm.github.io/downloads/papers/GeNeMe_2009.pdf). In Proceedings of the Workshop on Gemeinschaften in Neuen Medien (**GeNeMe'09"""), pages 79-89, Dresden, Germany, September 2009. |
| 2009 | voice recognition | conf. paper | Thilo Stadelmann and Bernd Freisleben. ["**Unfolding Speaker Clustering Potential: A Biomimetic Approach**"](https://stdm.github.io/downloads/papers/ACMMM_2009.pdf). In Proceedings of the ACM International Conference on Multimedia (**ACMMM'09"""), pages 185-194, Beijing, China, October 2009. ACM. |
| 2009 | voice recognition | conf. paper | Thilo Stadelmann, Steffen Heinzl, Markus Unterberger, and Bernd Freisleben. ["WebVoice: A Toolkit for **Perceptual Insights into Speech Processing**"](https://stdm.github.io/downloads/papers/CISP_2009.pdf). In Proceedingsof the 2nd International Congress on Image and Signal Processing (**CISP'09**), pages 4358-4362, Tianjin, China, October 2009. |
| 2009 | SoA | conf. paper | Steffen Heinzl, Markus Mathes, Thilo Stadelmann, Dominik Seiler, Marcel Diegelmann, Helmut Dohmann, and Bernd Freisleben. ["The Web Service Browser: Automatic Client Generation and Efficient Data Transfer for Web Services"](https://stdm.github.io/downloads/papers/ICWS_2009.pdf). In Proceedings of the 7th IEEE International Conference on Web Services (**ICWS'09**), pages 743-750, Los Angeles, CA, USA, July 2009. IEEE Press. |
| 2009 | SoA | **journal paper** | Steffen Heinzl, Dominik Seiler, Ernst Juhnke, Thilo Stadelmann, Ralph Ewerth, Manfred Grauer, and Bernd Freisleben. ["**A Scalable Service-Oriented Architecture for Multimedia Analysis, Synthesis, and Consumption**"](https://stdm.github.io/downloads/papers/IJWGS_2009.pdf). **International Journal of Web and Grid Services**, 5(3):219-260, 2009. Inderscience Publishers. |
| 2008 | video analysis | workshop paper | Markus Mühling, Ralph Ewerth, Thilo Stadelmann, Bing Shi, and Bernd Freisleben. ["University of Marburg at TRECVID 2008: High-Level Feature Extraction"](https://stdm.github.io/downloads/papers/TRECVID_2008.pdf). In Proceedings of TREC Video Retrieval Evaluation Workshop (**TRECVid'08**). [Available online, 2008](http://www-nlpir.nist.gov/projects/tvpubs/tv.pubs.org.htm). |
| 2007 | video analysis | workshop paper | Markus Mühling, Ralph Ewerth, Thilo Stadelmann, Bing Shi, Christian Zöfel, and Bernd Freisleben. ["University of Marburg at TRECVID 2007: Shot Boundary Detection and High-Level Feature Extraction"](https://stdm.github.io/downloads/papers/TRECVID_2007.pdf). In Proceedings of TREC Video Retrieval Evaluation Workshop (**TRECVid'07**). [Available online, 2007](http://www-nlpir.nist.gov/projects/tvpubs/tv.pubs.org.htm). |
| 2007 | video analysis | conf. paper | Ralph Ewerth, Markus Mühling, Thilo Stadelmann, Julinda Gllavata, Manfred Grauer, and Bernd Freisleben. ["Videana: A Software Toolkit for Scientific Film Studies"](https://stdm.github.io/downloads/papers/DTiMS_2007.pdf). In Proceedings of the **International Workshop on Digital Tools in Film Studies**, pages 1-16, Siegen, Germany, 2007. Transcript Verlag. |
| 2007 | video analysis | conf. paper | Markus Mühling, Ralph Ewerth, Thilo Stadelmann, Bernd Freisleben, Rene Weber, and Klaus Mathiak. ["**Semantic Video Analysis for Psychological Research on Violence in Computer Games**"](https://stdm.github.io/downloads/papers/CIVR_2007.pdf). In Proceedings of the ACM International Conference on Image and Video Retrieval (**CIVR'07**), pages 611-618, Amsterdam, The Netherlands, July 2007. ACM. |
| 2006 | video analysis | workshop paper | Ralph Ewerth, Markus Mühling, Thilo Stadelmann, Ermir Qeli, Björn Agel, Dominik Seiler, and Bernd Freisleben. ["University of Marburg at TRECVID 2006: Shot Boundary Detection and Rushes Task Results"](https://stdm.github.io/downloads/papers/TRECVID_2006.pdf). In Proceedings of TREC Video Retrieval Evaluation Workshop (**TRECVid'06**). [Available online, 2006](http://www-nlpir.nist.gov/projects/tvpubs/tv.pubs.org.htm). | 
| 2006 | voice recognition| conf. paper | Thilo Stadelmann and Bernd Freisleben. ["**Fast and Robust Speaker Clustering** Using the Earth Mover's Distance and MixMax Models"](https://stdm.github.io/downloads/papers/ICASSP_2006.pdf). In Proceedings of the 31st IEEE International Conference on Acoustics, Speech, and Signal Processing (**ICASSP'06**), volume 1, pages 989-992, Toulouse, France, April 2006. IEEE. |
| 2005 | video analysis | workshop paper | Ralph Ewerth, Christian Behringer, Tobias Kopp, Michael Niebergall, Thilo Stadelmann, and Bernd Freisleben. ["University of Marburg at TRECVID 2005: Shot Boundary Detection and Camera Motion Estimation Results"](https://stdm.github.io/downloads/papers/TRECVID_2005.pdf). In Proceedings of TREC Video Retrieval Evaluation Workshop (**TRECVid'05**). [Available online, 2005](http://www-nlpir.nist.gov/projects/tvpubs/tv.pubs.org.htm). |
| 2004 | voice recognition | diploma thesis | Thilo Stadelmann. ["Sprechererkennung in Videos"](https://stdm.github.io/downloads/papers/DiplomaThesis_2004.pdf). Diplomarbeit, Fachhochschule Giessen-Friedberg, 2004. |
