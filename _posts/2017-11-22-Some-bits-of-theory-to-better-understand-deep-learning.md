---
layout: post
title: Some bits of theory to better understand deep learning
---

This is a collection of links to some interesting recent theoretical advances to better understand deep learning. It is not complete, not even comprehensive. It is more of a reading list for the upcoming Christmas holidays. More on the topic can be found in [this](https://www.researchgate.net/project/Theories-of-Deep-Learning) new MOOC by Stanford Staff Hatef Monajemi, David Donoho and Vardan Papyan.

#### Insights from physics

* [Paper](https://arxiv.org/abs/1608.08225) by Lin, Tegmark and Rolnick

* [Summary](https://www.technologyreview.com/s/602344/the-extraordinary-link-between-deep-neural-networks-and-the-nature-of-the-universe/) on Technology Review

#### Insights from information theory

* [Paper 1](https://arxiv.org/abs/1703.00810) and [paper 2](https://arxiv.org/abs/1503.02406) by Naftali Tishby and colleagues

* [Summary](https://theneuralperspective.com/2017/03/24/opening-the-black-box-of-deep-neural-networks-via-information/) on The Neural Perspective

* The [talk](https://www.youtube.com/watch?v=bLqJHjXihK8) start started the buzz

#### Insights from neuroscience

* [Paper](http://www.cell.com/cell/comments/S0092-8674(17)30538-X) by Chang & Tsao

* My summary: The paper shows that monkey brains decode faces into ~200 orthogonal axes of facial appearance features, and that each face is recognized not by a single neuron (i.e., a softmax layer), but by a specific firing pattern of these 200 neurons. The monkey brain thus learns a face _embedding_. It is argued that this is similar to how CNNs learn representations, and that the discovery of the same mechanism in the brain might hint at a general underlying mechanism (_“The fact that the CNN developed these properties even though it was not explicitly trained to extract appearance coordinates suggests that an axis representation may arise naturally from general constraints on efficient face recognition.”_). The paper concludes with the following paragraph that cites Lin & Tegmark (see “physics” above) and hints at Hinton’s new Capsule Networks (see below): _“Our finding that AM cells are coding axes of shape-free appearance representations rather than ‘‘Eigenface’’ features (Figure 4L) is consistent with a recently proposed explanation for the effectiveness of deep neural networks in image recognition (Lin and Tegmark, 2016): a visual image on the retina can be considered the result of a hierarchical generative model starting from a set of simple variables, e.g., shape-free appearance features. Deep neural networks are reversing this generative hierarchy, one step at a time, to derive these variables at the final layers. According to this view, the reason the brain codes shape and appearance features is that these are the key input variables to the hierarchical generative model for producing face images that the brain has learned to reverse.”_

#### Insights from Geoffrey Hinton

* [Paper 1](https://openreview.net/pdf?id=HJWLfGWRb) and [paper 2](https://arxiv.org/abs/1710.09829) on capsule networks

* [Summary](https://medium.com/ai%C2%B3-theory-practice-business/understanding-hintons-capsule-networks-part-i-intuition-b4b559d1159b) by Max Pechyonkin
