---
title: 'The role of novel ideas in neural network research &#038; applications'
layout: post
date: 2016-12-14
category: research, reasons for the rise of deep learning
---

Public opinion has it that the current success of deep learning is built upon ideas from the 1970s and 1980s, enhanced by the availability of (a) increased computational power and (b) &#8220;big&#8221; data. Some add that a few minor algorithmic improvements also have been involved (e.g. <a href="https://arxiv.org/abs/1511.06856" target="_blank">BatchNorm</a> weight initialization [see also explanation <a href="http://www.computervisionblog.com/2016/06/deep-learning-trends-iclr-2016.html" target="_blank">here</a>], <a href="https://www.cs.toronto.edu/~hinton/absps/reluICML.pdf" target="_blank">ReLU</a> [rectified linear unit] nonlinearities, <a href="https://www.cs.toronto.edu/~hinton/absps/JMLRdropout.pdf" target="_blank">dropout</a> regularization, or the <a href="https://arxiv.org/abs/1412.6980" target="_blank">ADAM</a> optimizer). Building deep neural networks, the legend goes on, then boils down to clever engineering of the knobs and faders of these &#8220;black boxes&#8221;; and nobody really understands why they work or how they produce results: Pure black magic at worst, empiricism instead of science at best.

A prime example, on first glance, seems be Google&#8217;s <a href="https://research.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html" target="_blank">famous</a> inception <a href="https://arxiv.org/pdf/1409.4842v1.pdf" target="_blank">architecture</a>: A very wide & deep CNN that won the <a href="http://image-net.org/challenges/LSVRC/2014/" target="_blank">ImageNet ILSVRC&#8217;14 competition</a> by using an ensemble of 7(!) 22-layer(!) networks. Sounds like raw computational power (as ownly Google can have it), thrown at a huge pile of data, and thus winning by brute force.

But public opinion is not always right.

The original <a href="https://arxiv.org/pdf/1409.4842v1.pdf" target="_blank">inception</a> paper* from Google has this sentence: <strong><em>&#8220;[M]ost of this progress is not just the result of more powerful hardware, larger datasets and bigger models, but mainly a consequence of new ideas, algorithms and improved network architectures&#8221;</em></strong>. It goes on to show how how the merger of two beautiful ideas resulted in a network that is very deep & wide, but sparsly connected and explicitly designed to run on small-scale hardware (mobile phones) by exploiting considerably <em>less</em> parameters as competitive standard CNNs. These ideas are as follows:

  * A convolutional kernel in a CNN layer can be viewed as a small &#8220;model within the larger neural network model&#8221;, that basically resembles a generalized linear model (GLM). It is linear, thus limited in expressiveness. <a href="https://arxiv.org/pdf/1312.4400v3.pdf" target="_blank">This paper</a> explored the idea of replacing the typical GLM with an embedded neural network of its own, and gave positive results.
  * Quite some myths surround the challenge of finding the correct network architecture, given a specific problem. <a href="http://jmlr.org/proceedings/papers/v32/arora14.pdf" target="_blank">This</a> purely theoretical work (remarkably, a collaboration of academia and industry &#8211; so much for the boundaries of &#8220;applied science&#8221;) showed a way to iteratively (layer by layer) construct the best architecture by exploting local correlation structure of neurons firing together; only those neurons are then wired together that typically fire together (this goes back to <a href="https://en.wikipedia.org/wiki/Hebbian_theory" target="_blank">Donald Hebb&#8217;s research in neuroscience</a>).

This shows beautifully how at the core of recent deep learning successes there are indeed fundamentally new ideas, well backed up in theory and <a href="http://www.iro.umontreal.ca/~bengioy/talks/Brains+Bits-NIPS2016Workshop.pptx.pdf" target="_blank">even biologically plausible</a>. I conclude that we should let go of the following 3 urban legends:

  * neural networks being black boxes
  * their succes being a suprise, brought by mere clever engineering and brute force
  * their &#8220;making them work&#8221; being alchemy (<a href="https://www.zhaw.ch/de/ueber-uns/person/tugg/" target="_blank">Lukas Tuggener</a>&#8216;s term) or again brute force

Or, as <a href="https://www.quora.com/profile/Ismail-Elezi" target="_blank">Ismail Elezi</a> put it: _&#8220;We are getting closer to &#8216;we don&#8217;t understand how deep learning works&#8217; becoming a total false statement&#8221;_.

*) Great additional explanations of the inner workings of the inception module are found <a href="https://hackathonprojects.wordpress.com/2016/09/25/inception-modules-explained-and-implemented/" target="_blank">here</a>; if you wonder about the 1&#215;1 convolution, check <a href="http://stats.stackexchange.com/questions/194142/what-does-1x1-convolution-mean-in-a-neural-network" target="_blank">here</a>.