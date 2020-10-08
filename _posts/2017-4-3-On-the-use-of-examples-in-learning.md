---
layout: post
title: On the use of examples in learning
date: 2017-04-03
modified: 2017-04-03
category: education, teaching, theory vs. practice
comments: true
---

Once in a while in a discussion on education or science, the topic of the perceived opposition of theory and practice comes up. It is usually raised by one party with a strong view on either a theory- or an application focus, with the goal of discrediting the other viewpoint: _"This is just theory (and thus worthless), because what we need is to make it run"_. In a classroom setting, you sometimes hear it from students complaining about too much abstract knowledge and too less examples.

<!-- more -->

The same argument is also used the other way round. I came to the conclusion that both is shortsighted thinking, robbing the holder of such a viewpoint from the very benefit the other view can grant him or her. Let me explain this using the example of the classroom setting above, and using an analogy from machine learning:


In a supervised classification setting in machine learning, you provide an algorithm with samples of possible input data, together with the expected output per data point (a “class label”). The goal of the machine learning algorithm is to come up with an internal model (also called a “theory”) that generalizes beyond the concrete input-output tuples it has seen, to previously unseen data. In fact, the only way such a model can ever be useful is if it can generalize:

Suppose you want to build a classifier that [takes pictures of cats and dogs as input, and learns to tell these two classes apart](https://www.kaggle.com/c/dogs-vs-cats). Even if you have collected the vast amount of one million pictures of cats and one million pictures of dogs, you are not impressed if the learned model works well on these two million training cases. You want it to succeed on the newly taken picture of your friend’s cat.

To ensure that this generalization happens, in machine learning we use a second data set beyond the two million pictures in the abovementioned training set: after finishing the training of our model, we provide it with a _test set of examples_ of cat and dog images that the algorithm has never seen before, and measure its classification accuracy on it. This gives us insight into how well the learned model (theory) is applicable in practice.

Back to the classroom. No student is interested in examples _per se_. Rather, each student is interested in applicable knowledge that helps him or her to solve problems of some practical relevance. And for knowledge to be applicable to unseen situations (i.e., to generalize well), it has to reside in one’s brain as _abstract_ knowledge: knowledge that is independent of any concrete constraints to be _transferable_ to a newly arising task. (Yes, examples are also transferable by means of [transduction](https://en.wikipedia.org/wiki/Transduction_(machine_learning)), but humans by far more often and also better use the principle of [deduction](https://en.wikipedia.org/wiki/Deductive_reasoning) to apply knowledge to new examples.)

So what, then, is the use of examples in learning? The same as in machine learning: they serve as a means for the student to check if the internalized abstract knowledge works well on unseen examples – i.e., if it has been understood correctly. This is a very important function – but playing off theory and examples against each other is a little bit like [wagging the dog](https://www.youtube.com/watch?v=CNo0BicRM8k). 

(And yes, of course learning can also happen by going through quite an amount of examples and abstract them down to a theory on your own. That is what is done in the [inductive](https://en.wikipedia.org/wiki/Inductive_reasoning) machine learning case above, and this is how humans learn most things in life. But like inductive ML only reached impressive results in the [big data era](https://www.slideshare.net/thilo_stadelmann/der-wert-von-daten-in-zeiten-von-big-data) of plenty of available examples, so does inductive human learning take years. Usually we try to shortcut these in education.)
