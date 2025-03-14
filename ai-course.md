---
title: AI course
layout: page
comments: true
---

This is the companion website to my one semester course on Artificial Intelligence. The course used to be part of the bachelor of computer science curriculm at ZHAW School of Engineering as the elective course "KI1" during the last year of study. It reflects the status quo as of fall term 2018 (and has been extended into numerous modules detailing certain aspects of machine learning and agent design by now). You can find the underlying didactic concept [here](https://stdm.github.io/ATLAS/) and [here](https://stdm.github.io/Science-applied/) (in German).

### TOC
1. [Syllabus](#syllabus)
2. [Resources](#resources)
3. [Educational objectives](#objectives)
4. [Prerequisites](#prerequisites)


[<img alt="Lecturing" src="http://stdm.github.io/images/ai-recording.jpg"/>](http://stdm.github.io/images/ai-recording.jpg)


<a name="syllabus"></a>  
## Syllabus

| Topic | Lecture (videos in German) | Lab | AIMA book |
| --- | --- | --- | --- |
| **Introduction** | [V01: Introduction](http://stdm.github.io/downloads/courses/AI/V01_Introduction.pdf) ([a](https://youtu.be/tvN09avji_Y), [b](https://youtu.be/93A9-nyMBVE)) | [P01: Reading assignment](http://stdm.github.io/downloads/courses/AI/P01_ReadingAssignment.zip) | ch. 1 |
| | [V02: Intelligent agents](http://stdm.github.io/downloads/courses/AI/V02_IntelligentAgents.pdf)	([a](https://youtu.be/YKe-XPa2r-s), [b](https://youtu.be/5oB9TmzflQc)) | [P02: 2048 game playing agent](http://stdm.github.io/downloads/courses/AI/P02_2048.zip) | ch. 2 |
| **Search** | [V03: Problem solving through search](http://stdm.github.io/downloads/courses/AI/V03_ProblemSolvingThroughSearch.pdf) ([a](https://youtu.be/ozgIDsWvRVU), [b](https://youtu.be/naOEvcKT77g)) | | ch. 3 |
| | [V04: Local and adversarial search](http://stdm.github.io/downloads/courses/AI/V04_LocalAndAdversarialSearch.pdf) ([a](https://youtu.be/pLquR8LvWJ4), [b](https://youtu.be/Y9K7b0k5kxo)) | | ch. 5 (+4) |
| | [V05: Constraint satisfaction problems](http://stdm.github.io/downloads/courses/AI/V05_ConstrainSatisfactionProblems.pdf) ([a](https://youtu.be/q_I3FuSQTiE), [b](https://youtu.be/7m_o0X2zvog))	| [P03: Constraint satisfaction problems & Datalog](http://stdm.github.io/downloads/courses/AI/P03_CSP_Datalog.zip) | ch. 6 |
| **Planning** | [V06a: Knowledge, reasoning & logic](http://stdm.github.io/downloads/courses/AI/V06a_KnowledgeReasoningLogic.pdf) ([a](https://youtu.be/aCJ7mJRQnCY), [b](https://youtu.be/xgIBhrtMe_w)) | (in-class: [P03b: Logic exercises](http://stdm.github.io/downloads/courses/AI/P03b_LogicExercises.pdf)) | ch. 7 |
| | [V06b: Datalog](http://stdm.github.io/downloads/courses/AI/V06b_Datalog.pdf) ([a](https://youtu.be/hfKdL0igVjk), [b](https://youtu.be/qEPfKtEypes)) | | ch. 8 (+9) |
| | [V07: Planning](http://stdm.github.io/downloads/courses/AI/V07_Planning.pdf) ([a](https://youtu.be/g5AShEMANRA), [b](https://youtu.be/Dfc2QHGgO8k)) | | ch. 10 (+11) |
| **Learning** | [V08: Learning agents](http://stdm.github.io/downloads/courses/AI/V08_LearningAgents.pdf) ([a](https://youtu.be/G1xk4-s4XT8), [b](https://youtu.be/rAXGU-KI9UU))	| [P04: Decision trees](http://stdm.github.io/downloads/courses/AI/P04_DecisionTrees.zip) | ch. 18.1-18.6 |
| | [V09: Ensemble learning](http://stdm.github.io/downloads/courses/AI/V09_EnsembleLearning.pdf) ([a](https://youtu.be/YLNzeJjNSW0), [b](https://youtu.be/6RwTjMDLwA8)) | | ch. 18.10-18.12 |
| | [V10: Probabilistic learning](http://stdm.github.io/downloads/courses/AI/V10_ProbabilisticLearning.pdf)	([a](https://youtu.be/T0TWEuNKJ0I), [b](https://youtu.be/DEh2HriZGUo)) | [P05: Multimedia analysis](http://stdm.github.io/downloads/courses/AI/P05_MultimediaAnalysis.zip) | ch. 20 |
| **Selected chapters** | [V11: Generative modeling with neural nets](http://stdm.github.io/downloads/courses/AI/V11_NeuralGenerativeModeling.pdf) ([a](https://youtu.be/TLXBsmBBoAY), [b](https://youtu.be/KlOO7-FSeJU)) | (see [this blog post](https://stdm.github.io/Experimenting-with-generative-adversarial-nets/) for a code example) | ch. 18.7 |
| | [V12: AI & society](http://stdm.github.io/downloads/courses/AI/V12_SocietalImpact.pdf) ([a](https://youtu.be/aryGTsyS-Ic), [b](https://youtu.be/lYuFc3MLm9s))	| [P01b: Reading assignment, revisited](http://stdm.github.io/downloads/courses/AI/P01b_Revisited.zip) | ch. 26 |

All links lead to documents as of fall term 2018.

Additional material [optional]: 
- [AlphaZero: Learning games from selfplay](http://stdm.github.io/downloads/talks/2018-11-15_AlphaZero-LearningGamesFromSelfplay.pdf) ([video](https://youtu.be/_Z31-5D3RZg) in English)
- [Deep Learning in the wild](https://stdm.github.io/downloads/talks/2018-09-21_DL-in-the-wild.pdf) ([video](https://youtu.be/efCyLhSACoU) in English)
- [Was kann KI leisten?](https://stdm.github.io/downloads/talks/2019-03-07_Was-kann-KI-leisten.pdf) ([video](https://youtu.be/Vxsddc9bGUE) in German) as a 90 minutes long summary of this one-semester course

<a name="resources"></a>  
## Resources

**Current slides, lab descriptions, terms & conditions:** see [OLAT](https://olat.zhaw.ch/auth/RepositoryEntry/219152410/CourseNode/95069693647358) (you can login as guest even without a ZHAW account).

**Video recordings:** see YouTube playlist for [fall 2018](https://www.youtube.com/watch?v=tvN09avji_Y&list=PLdUGLyqPtOZoaW4xBWMpDA37vIlbsh2xY) term as well as [this video](https://youtu.be/_zLktk63ezM) for exam preparation.

**Audio-only recordings:** see Collecture for [fall 2017](https://collecture.io/groups/65dda3ed-4946-4f40-8af8-ba55e964b140?autosub=true) and [spring 2017](https://collecture.io/groups/99275ecf-ae1a-4aaa-8375-0f484fa352ef?autosub=true) terms.

**Book:** Russell, Norvig, ["Artificial Intelligence - A Modern Approach"](http://aima.cs.berkeley.edu/), 3rd Edition, Pearson, 2010.


<a name="objectives"></a>  
## Educational objectives

1. You know the breadth of AI problem solving strategies
  * ...thus identify such challenges in practice
  * ...and develop corresponding solutions on your own.
2. You can explain the discussed algorithms and methodologies
  * ...and are able to transfer it to the real world.

**What is it all about?** Computer opponents in games, fastest route in navigation devices, optimized flight schedules, decision support in hospitals, design of pharmaceutical proteins to fight cancer - the foundation of all these fascinating application is "Artificial Intelligence" (AI).

**Why is it relevant?** Since the 1960s, AI is about developing solutions for complex problems that could formerly only be solved by humans. AI is a classical subdiscipline of computer science. Its methods are so universally used that our text book for this course is among the 25 most-cited scientific publications on Citeseer!

**Who should attend?** This is a very much practice-oriented course on selected foundations of AI and Machine Learning (ML), aiming at hands-on problem solving competency for everyday software challenges. It is geared towards everyone who is curious for smart software and is especially relevant for software engineers, would-be data scientists and as a foundation for further interdisciplinary studies in areas like information engineering, speech processing, computer vision or robotics.

  
<a name="prerequisites"></a>  
## Prerequisites

Successfully completed assessment phase (i.e., foundations of computer science: good command of programming, linear algebra, probability, algorithms & data structures), affinity towards algorithms, enjoying the topic.