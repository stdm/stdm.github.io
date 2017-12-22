---
layout: post
title: Some bits of theory to better understand deep learning
---

This is a collection of links to some interesting recent theoretical advances in order to better understand deep learning. It is not complete, not even comprehensive. It is more of a reading list for the upcoming Christmas holidays. More on the topic of deep learning theory can be found in [this](https://www.researchgate.net/project/Theories-of-Deep-Learning) new MOOC by Stanford professors Hatef Monajemi, David Donoho and Vardan Papyan, and in [this overview blogpost](https://medium.com/mlreview/modern-theory-of-deep-learning-why-does-it-works-so-well-9ee1f7fb2808) by Dmytrii S. on why deep neural nets generalze so well.

### Insights from physics

Lin, Tenmark and Rolnick (2016) argue that in physics, most complex phenomena are explained using simple models and formulas; this might explain why deep neural nets learn so well despite the vast complexity of the tasks.

* [Paper](https://arxiv.org/abs/1608.08225) from the Journal of Statistical Physics

* [Summary](https://www.technologyreview.com/s/602344/the-extraordinary-link-between-deep-neural-networks-and-the-nature-of-the-universe/) on Technology Review

### Insights from information theory

Naftali Tishby and colleagues argue that neural nets learn in two distinct phases: first (and quickly), they coarsly fit the labels using the data, and then (longer) they learn to generalize by compressing the noisy data representation. We are proud to have Prof. Tishby giving a keynote on this topic at [SDS 2018](http://www.sds2018.ch), the 5th Swiss Conference on Data Science!

* [Paper 1](https://arxiv.org/abs/1703.00810) and [2](https://arxiv.org/abs/1503.02406) on arXiv

* [Summary](https://theneuralperspective.com/2017/03/24/opening-the-black-box-of-deep-neural-networks-via-information/) on The Neural Perspective ([here](https://www.quantamagazine.org/new-theory-cracks-open-the-black-box-of-deep-learning-20170921/)'s also a more intuitive one)

* Tishby's [talk](https://www.youtube.com/watch?v=bLqJHjXihK8) that started the discussion

### Insights from neuroscience

Chang and Tsao show that monkey brains decode faces into ca. 200 orthogonal axes of facial appearance features, and that each face is recognized not by a single neuron (i.e., a softmax layer), but by a specific firing pattern of these 200 neurons. The monkey brain thus learns a face _embedding_. 

* [Paper](http://www.cell.com/cell/comments/S0092-8674(17)30538-X) from Cell Journal

* My summary: It is argued that this encoding procedure of the monkey brain is similar to how CNNs learn representations, and that the discovery of the same mechanism in the brain might hint at a general underlying mechanism (_"The fact that the CNN developed these properties even though it was not explicitly trained to extract appearance coordinates suggests that an axis representation may arise naturally from general constraints on efficient face recognition."_). The paper concludes with the following paragraph that cites Lin & Tegmark (see “physics” above) and hints at Hinton’s new Capsule Networks (see below): _"Our finding that AM cells are coding axes of shape-free appearance representations rather than ''Eigenface'' features (Figure 4L) is consistent with a recently proposed explanation for the effectiveness of deep neural networks in image recognition (Lin and Tegmark, 2016): a visual image on the retina can be considered the result of a hierarchical generative model starting from a set of simple variables, e.g., shape-free appearance features. Deep neural networks are reversing this generative hierarchy, one step at a time, to derive these variables at the final layers. According to this view, the reason the brain codes shape and appearance features is that these are the key input variables to the hierarchical generative model for producing face images that the brain has learned to reverse."_

### Insights from Geoffrey Hinton

Geoffrey Hinton published an improvement of the errors he founds in current CNNs (max pooling, need for many training exaples): capsule networks. They are able to learn hierarchies of representations with respect to their relation to each opther (e.g., in computer vision: translation and rotation). This makes it much easier for the network to learn that objects depicted from different viewpoints are actually the same thing (i.e., CapsNets need less training data).

* [Paper 1](https://openreview.net/pdf?id=HJWLfGWRb) and [2](https://arxiv.org/abs/1710.09829) on arXiv

* [Summary](https://medium.com/ai%C2%B3-theory-practice-business/understanding-hintons-capsule-networks-part-i-intuition-b4b559d1159b) by Max Pechyonkin

### Insights from Bayesian theory

Yarin Gal and colleagues argues that using dropout in the evaluation phase of a deep net (thus effectively executing slightly different versions of the same net on exactly the same test data), and then creating a statistic of the prediction probabilities for all classes, helps in judging if the network can classify a certain example well, or if it in fact has no clue what the current input is (this might happen if you train a network on all dogs and then show it a cat in evaluation: it will classify the cat as some dog, maybe even with high probability, because it does not have the option to say "I don't know").

* [Paper](https://arxiv.org/abs/1506.02142) on arXiv

* [Summary](http://mlg.eng.cam.ac.uk/yarin/blog_3d801aa532c1ce.html) on the autor's own blog
