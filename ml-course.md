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


[<img alt="lecturing" src="http://stdm.github.io/images/AlphaZero.jpg"/>](http://stdm.github.io/images/AlphaZero.jpg)


<a name="syllabus"></a>  
## Syllabus

| **Topic** | **Lecture (& videos)** | **Lab** | **Self study** | **Lecturer** |
| **Preparation** |  |  | P01.1-5 | |
| **Introduction** | [V01: Introduction](https://stdm.github.io/downloads/courses/ML/V01_Introduction.pdf) ([a](https://youtu.be/A2vd0kwjnBI), [b](https://youtu.be/GeJu8bRXvyM)) | [P01: Discuss ML fundamentals](https://stdm.github.io/downloads/courses/ML/P01_ReadingAssignment_1.pdf) | P01.6-7 | stdm |
| | V02: Formulating learning problems | P02.1: Linear regression from scratch | | stdm |
| **Supervised learning** | V03: Model assessment & selection | P04.1: Analyzing cross validation| P03 | stdm |
| | V04: SVMs | P04.2: SVM in IPython | | stdm |
| | V05: Ensembles | P04.3: Ensembles in practice | P05 | stdm |
| | V06.3: Debugging ML algorithms; <br> V07.1: System development - what to give priority to? | P06.2: Applying learning curves | Raschka ch. 6; P07 | wuerc |
| | V08: Feature engineering | Lab08 | | wuerc |
| | V09a: Probabilistic reasoning, Gaussian distribution and Bayes' theorem | Lab09a | 09a reader | wuerc |
| | V09b: Gaussian processes | Lab09b | Do, 2017 | wuerc |
| **Unsupervised learning** | V10: Dimensionality reduction | Lab10 | Raschka ch. 5 | wuerc |
| | V11: Clustering | Lab11 | Raschka ch. 11; Ng | wuerc |
| **Selected chapters** | V12a: Learning games from selfplay | P12: Selfplay for Tic-Tac-Toe | | stdm |

All links lead to documents as of soring term 2019.

Additional material [optional]: 
- [Deep Learning in the wild](https://stdm.github.io/downloads/talks/2018-09-21_DL-in-the-wild.pdf) ([video](https://youtu.be/efCyLhSACoU) in English)


<a name="resources"></a>  
## Resources

**Current slides, lab descriptions, terms & conditions:** see [Moodle](https://moodle.msengineering.ch/course/view.php?id=1076) (you need a valid account as an inscribed student).

**Video recordings:** see YouTube playlist for [fall 2019](https://www.youtube.com/playlist?list=PLdUGLyqPtOZp1oAg-8MRlmIsveW3NE8SQ).

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