---
title: ML course
layout: page
comments: true
---

This is the companion website to my one semester course on machine learning, co-taught with [Prof. Christoph Wuersch](https://www.ntb.ch/mitarbeiter/christoph-wuersch/) from the NTB Buchs. The course is part of the [Master of Science in Engineering](https://www.msengineering.ch/en/home.html) (MSE) program in computer science and data science, offered collaboratively by the engineering faculties of the Swiss universities of applied sciences. This website reflects the status quo as of spring term 2019.

### TOC
1. [Syllabus](#syllabus)
2. [Resources](#resources)
3. [Educational objectives](#objectives)
4. [Prerequisites](#prerequisites)


[<img alt="lecturing" src="http://stdm.github.io/images/TSM_MachLe.jpg"/>](http://stdm.github.io/images/TSM_MachLe.jpg)


<a name="syllabus"></a>  
## Syllabus

| **Topic** | **Lecture (& videos)** | **Lab** | **Self study** | **Lecturer** |
| **Preparation** |  |  | [P01.1-5](https://stdm.github.io/downloads/courses/ML/P01_ReadingAssignment_1.pdf) | |
| **Introduction** | [V01: Introduction](https://stdm.github.io/downloads/courses/ML/V01_Introduction.pdf) ([a](https://youtu.be/A2vd0kwjnBI), [b](https://youtu.be/GeJu8bRXvyM)) | [P01: Discuss ML fundamentals](https://stdm.github.io/downloads/courses/ML/P01_ReadingAssignment_1.pdf) | [P01.6-7](https://stdm.github.io/downloads/courses/ML/P01_ReadingAssignment_1.pdf) | stdm |
| | [V02: Formulating learning problems](https://stdm.github.io/downloads/courses/ML/V02_FormulatingLearningProblems.pdf) ([code](https://stdm.github.io/downloads/courses/ML/V02_FormulatingLearningProblems_Code.zip)) ([a](https://youtu.be/Nng1kJIEJdg), [b](https://youtu.be/9migPdNMPA8)) | [P02.1: Linear regression from scratch](https://stdm.github.io/downloads/courses/ML/P02_MachineLearningFromScratch.zip) | | stdm |
| **Supervised learning** | [V03: Model assessment & selection](https://stdm.github.io/downloads/courses/ML/V03_ModelAssessment_and_Selection.pdf) ([a](https://youtu.be/wdKWlV4za_k), [b](https://youtu.be/WpyNmBtYbZ4)) | [P04.1: Analyzing cross validation](https://stdm.github.io/downloads/courses/ML/P04_SVM_ModelSelection.zip) | [P03](https://stdm.github.io/downloads/courses/ML/P03_ReadingAssignment_2.pdf) | stdm |
| | [V04: SVMs](https://stdm.github.io/downloads/courses/ML/V04_SVMs.pdf) ([a](https://youtu.be/QhGa8FkSgz0), [b](https://youtu.be/GvO7_Pt2I-o)) | [P04.2: SVM in IPython](https://stdm.github.io/downloads/courses/ML/P04_SVM_ModelSelection.zip) | | stdm |
| | [V05: Ensembles](https://stdm.github.io/downloads/courses/ML/V05_EnsembleMethods.pdf) ([a](https://youtu.be/AYyIWzFc_9I), [b](https://youtu.be/l6n53cGLB9c)) | [P04.3: Ensembles in practice](https://stdm.github.io/downloads/courses/ML/P04_SVM_ModelSelection.zip) | [P05](https://stdm.github.io/downloads/courses/ML/P05_ReadingAssignment_3.pdf) | stdm |
| | [V06: Bias-variance-tradeoff: crossvalidation & learning curves](https://stdm.github.io/downloads/courses/ML/V06_BiasVariance-LearningCurves.pdf) ([a](https://youtu.be/ILesIecBcjA), [b](https://youtu.be/DYwYgYrt_OA), [c](https://youtu.be/NH1xP0I0_3Q)) <br><br> [V07.1: System design: what to give priority to](https://stdm.github.io/downloads/courses/ML/V07_SystemDesign.pdf) | [P06.2: Applying learning curves](https://stdm.github.io/downloads/courses/ML/P06_Diagnostic.zip) | [further reading](https://stdm.github.io/downloads/courses/ML/V06_further-reading.txt) | wuerc |
| | [V08: Feature engineering](https://stdm.github.io/downloads/courses/ML/V08_FeatureEngineering.pdf) ([a](https://youtu.be/ucdHa6_Lexw), [b](https://youtu.be/ZYDKPC-xePA), [c](https://youtu.be/CfhKAOU9HUw)) | [Lab 8](https://stdm.github.io/downloads/courses/ML/Lab8_FeatureEngineering.zip) | [further reading](https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html) | wuerc |
| | [V09a: Probabilistic reasoning, Gaussian distribution and Bayes' theorem](https://stdm.github.io/downloads/courses/ML/V09a_BayesTheorem.pdf) ([a](https://youtu.be/9R8lGPxuuuM), [b](https://youtu.be/iYTwegjFKPc), [c](https://youtu.be/7KVgPf3olEg)) | [Lab 9a](https://stdm.github.io/downloads/courses/ML/Lab9a_ProbabilisticReasoning.zip) | [further reading](https://stdm.github.io/downloads/courses/ML/V9a_further-reading.txt) | wuerc |
| | [V09b: Gaussian processes](https://stdm.github.io/downloads/courses/ML/V09b_GaussianProcesses.pdf) ([a](https://youtu.be/mcwTIPqNd6Y), [b](https://youtu.be/lcQLYn8sSkM), [c](https://youtu.be/JTl1zrQCu2Q)) | [Lab 9b](https://stdm.github.io/downloads/courses/ML/Lab9b_GaussianProcesses.zip) ([d](https://youtu.be/bw2PIEpfzWA), [e](https://youtu.be/TyK1zkE-HAo)) | optional [further reading](https://see.stanford.edu/materials/aimlcs229/cs229-gp.pdf) | wuerc |
| **Unsupervised learning** | [V10: Dimensionality reduction](https://stdm.github.io/downloads/courses/ML/V10_DimensionalityReduction.pdf) ([a](https://youtu.be/jdkxll92g-Y), [b](https://youtu.be/WEOO_6rFWuU), [c](https://youtu.be/rp4_6N61jE4)) | [Lab 10](https://stdm.github.io/downloads/courses/ML/Lab10_DimensionalityReduction.zip) | optional [further reading](https://stdm.github.io/downloads/courses/ML/V10_further-reading.txt) | wuerc |
| | [V11: Clustering]() ([a](https://youtu.be/JTloiokrEpo), [b](https://youtu.be/oOycsuDsPkI)) | [Lab 11](https://stdm.github.io/downloads/courses/ML/Lab11_Clustering.zip) | [further reading](https://stdm.github.io/downloads/courses/ML/V11_further-reading.txt) | wuerc |
| **Selected chapters** | V12a: Learning games from selfplay | P12: Selfplay for Tic-Tac-Toe | | stdm |

All links lead to documents as of spring term 2019.

Additional material [optional]: 
- [Deep Learning in the wild](https://stdm.github.io/downloads/talks/2018-09-21_DL-in-the-wild.pdf) ([video](https://youtu.be/efCyLhSACoU) in English)
- [Was kann KI leisten?](https://stdm.github.io/downloads/talks/2019-03-07_Was-kann-KI-leisten.pdf) ([video](https://youtu.be/Vxsddc9bGUE)] in German) as a 90 minutes long summary of this one-semester course


<a name="resources"></a>  
## Resources

**Current slides, lab descriptions, terms & conditions:** see [Moodle](https://moodle.msengineering.ch/course/view.php?id=1076) (you need a valid account as an inscribed student).

**Video recordings:** see YouTube playlist for [spring 2019](https://www.youtube.com/playlist?list=PLdUGLyqPtOZp1oAg-8MRlmIsveW3NE8SQ).

**Audio-only recordings:** see Collecture for [spring 2018](https://collecture.io/groups/7325878c-845f-4827-8e1c-3f7c15092f4a?autosub=true) recordings (you need to create a free account).

**Books:**

- T. Mitchell, ["Machine Learning"](http://www.cs.cmu.edu/~tom/mlbook.html), 1997

- C. M. Bishop, "Pattern Recognition and Machine Learning", 2006

- G. James et al., ["An Introduction to Statistical Learning"](http://www-bcf.usc.edu/~gareth/ISL/), 2014

- K. P. Murphy, ["Machine Learning - A Probabilistic Perspective"](https://www.cs.ubc.ca/~murphyk/MLbook/), 2012

- S. Raschka, ["Python Machine Learning"](https://sebastianraschka.com/books.html), 2017 (2nd Edition)

- further [literature list](https://stdm.github.io/downloads/courses/ML/literature-guide.xlsx)


<a name="objectives"></a>  
## Educational objectives

1. Students **know** the **background and taxonomy** of machine learning methods.

2. On this basis, they **formulate** given problems as **learning tasks** and **select** a **proper learning method**.

3. Students are **able to convert** a data set into a proper **feature set** fitting for a task at hand.

4. They **evaluate** the chosen **approach** in a structured way using proper design of experiment.

5. Students **know how** to select models, and **"debug"** features and learning algorithms if results do not fit expectations.

6. Students are able to leverage on the evaluation framework to **tune the parameters** of a given system and **optimize** its performances.

7. Students **have seen examples of different data** sources / problem types and are **able to acquire additional expert knowledge** from the scientific literature.

Machine learning (ML) emerged out of artificial intelligence and computer science as the academic discipline concerned with "giving computers the ability to learn without being explicitly programmed" (A. Samuel, 1959). Today, it is the methodological driver behind the mega-trends of big data and data science. ML experts are highly sought after in industry and academia alike.

This course builds upon basic knowledge in math, programming and analytics/statistics as is typically gained in respective undergraduate courses of diverse engineering disciplines. From there, it teaches the foundations of modern machine learning techniques in a way that focuses on practical applicability to real-world problems. The complete process of building a learning system is considered:

- formulating the task at hand as a learning problem;

- extracting useful features from the available data;

- choosing and parameterizing a suitable learning algorithm.

Covered topics include cross-cutting concerns like ML system design and debugging (how to get intuition into learned models and results) as well as feature engineering; covered algorithms include (amongst others) Support Vector Machines (SVM) and ensemble methods.


<a name="prerequisites"></a>  
## Prerequisites

**Math**: basic calculus / linear algebra / probability calculus (e.g., derivatives, matrix multiplication, normal distribution, Bayes' theorem)

**Statistics**: basic descriptive statistics (e.g., mean, variance, co-variance, histograms, box plots)

**Programming**: good command of any structured programming language (e.g., Python, Matlab, R, Java, C, C++)

**Analytics**: basic data analysis methods (data pre-processing, decision trees, k-means clustering, linear & logistic regression)