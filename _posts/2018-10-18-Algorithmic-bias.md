---
title: 'Algorithmic bias: important topic, problematic term'
layout: post
date: 2018-10-18
modified: 2018-10-18
category: digitalization, ethics
comments: true
---

Recently, I engaged in a discussion within the [Expert Group on Data Ethics](https://data-service-alliance.ch/expertise/expert-groups) on the pros and cons of the term ["algorithmic bias"](https://en.wikipedia.org/wiki/Algorithmic_bias), which describes the fact that certain people groups might be discriminated by an automatic decision making system, and how to prevent this. While every research in this sphere is very important and rightly so at the forefront of current discussions in data science, artificial intelligence and digital ethics (see e.g. [here](https://arxiv.org/abs/1706.02409), [here](https://ieeexplore.ieee.org/document/5360534) or [here](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)), I think the term itself might do more harm than good in the public discussion. Here's my line of thought:

1. The (German) [definition of algorithm](https://de.wikipedia.org/wiki/Algorithmus) in computer science and beyond is very broad, pointing to any unambiguous sequence of instructions to solve a given problem; it can be implemented as a computer program that transforms some input into corresponding output. As this encompasses any automatic computer program, we are formally save to call any biased decision by a computer program "algorithmic bias".

_But maybe we can be more precise to prevent unnecessary harm; let me explain._

2. In computer science practice, we usually constraints the use of the word "algorithm" to only mean those programs that solve "a class of problems" instead of every customized piece of code (see also [English Wikipedia](https://en.wikipedia.org/wiki/Algorithm), first sentence). Those algorithms go by certain well-established names, e.g. the [Quicksort algorithm](https://en.wikipedia.org/wiki/Quicksort) to sort lists of items; the [Gauss-Newton algorithm](https://en.wikipedia.org/wiki/Gauss%E2%80%93Newton_algorithm) to solve non-linear least squares problems; the [Backpropagation algorithm](https://en.wikipedia.org/wiki/Backpropagation) to train neural nets; and so forth. This fits well with the terminology used in the machine learning community: If I solve a given problem (e.g., face detection) by tweaking the parameters of such a well-known algorithm, I publish about the _model_ that I built and its properties; if I fundamentally change the method by which I built the model, I publish a _new machine learning algorithm_ (which is often considered a more fundamental research result).

_Ok, whatever; what has the terminology in computer science to do with data ethics?_

3. I _suppose_ that the "general public" (that reads newspapers, votes, etc.) has a similar understanding: for the non-expert, our digital world/economy runs on algorithms – fundamental building blocks of the digital age, like e.g. Diesel engines in the mechanical / automotive world. They don't understand every ever written piece of code as a separate algorithm (as would be warranted by point [1] above); rather, they see algorithms as the general principles of computing (the view presented in [2] above), which produce specific results (that it is by means of an intermediate model is probably not well understood). Consider now the measure of fear, uncertainty and doubt we induce if we speak of "algorithmic bias": this conveys the message (to those having a view according to [2/3] above) that the pillars of the digital world are fundamentally flawed. not being able to handle anything in a fair manner – much like the FUD that has recently befallen those owning a Diesel car (the engine is beyond repair – what else can we do than look for something else?).

_Ok, if the possibility for this misunderstanding is valid, what can we do about it?_

4. We can completely overcome this problem if we are more precise and move from the general (and, as discussed, possibly misleading) term "algorithmic bias" to more specific forms like ["selection bias"](https://en.wikipedia.org/wiki/Selection_bias) (for the bias in us humans selecting the wrong algorithms/model for a specific task; or the wrong data for a dataset) or ["dataset bias"](http://people.csail.mit.edu/torralba/research/bias/) (for the case where a in principle neutral algorithm like any machine learning method creates a model that picks up biases in the data) etc. 

_Because in the end, all the bias introduced into computer programs ultimately comes from a human source (which can be mitigated), and it does not help to open up a new virtual, blurry front line against algorithmd/machines that [arouses emotions](https://en.wikipedia.org/wiki/Beeldenstorm) but does not bring us closer to a solution (of our human problems)._
