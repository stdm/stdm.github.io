---
id: 400
title: Experimenting with Generative Adversarial Nets
date: 2016-11-30T19:19:01+00:00
author: stdm
layout: post
guid: https://dublin.zhaw.ch/~stdm/?p=400
permalink: /?p=400
categories:
  - Education
  - Research
---
Recently, I got intrigued by so-called Generative Adversarial Nets or GANs (see <a href="https://arxiv.org/abs/1406.2661" target="_blank">the original paper</a>, <a href="https://arxiv.org/abs/1511.06434" target="_blank">the important improvement</a> to make it practical, an <a href="https://medium.com/@awjuliani/generative-adversarial-networks-explained-with-a-classic-spongebob-squarepants-episode-54deab2fce39#.x3strdv31" target="_blank">easy to underastand implementation</a> and a <a href="https://bamos.github.io/2016/08/09/deep-completion/" target="_blank">nice application</a> here). So much so that I derusted my <a href="https://gist.github.com/awjuliani/8ebf356d03ffee139659807be7fa2611#file-dcgan-ipynb" target="_blank">programming </a>and <a href="https://rumorscity.com/wp-content/uploads/2014/08/10-Best-VIM-Cheat-Sheet-04.jpg" target="_blank">linux command line operation</a> skills, learned <a href="https://www.dataquest.io/blog/docker-data-science/" target="_blank">docker</a>, and started playing around myself for the first time in several month.



<!--more-->

The video above shows in each frame (at 30 FPS) the result of synthesizing 6&#215;6 handwritten digits after 2 mini batches of training on <a href="http://yann.lecun.com/exdb/mnist/" target="_blank">MNIST data</a>. The 6&#215;6=36 z vectors have been drawn at random before the first mini batch and stay constant, so you can basically watch what the network learns to generate from a fixed deterministic input. The z dimension is kept very low at 2 (so you could in principle visualize the generated images directly in the 2D z space).

As can bee seen in the video, the untrained network in the beginning generates random noise images, then quickly changes to something drawing-like, and pretty quickly arrives at recognizable digits. But it takes some time to differentiate (i.e., generate different images for different z vectors), and the GAN (precisely: it&#8217;s G part) takes almost 3/4 of the overall 2&#215;50&#8217;000 mini batches to learn a representation that is so stable that for a fixed z the generated number stays basically the same and doesn&#8217;t alternate between different digits.

**Transfer to faces**

After the abovementioned code worked almost out of the box, I tried to change it to work for a different data set: faces from the <a href="http://vis-www.cs.umass.edu/lfw/" target="_blank">LFW database</a>. I only rewrote some code to load and preprocess the data from <a href="http://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_lfw_people.html" target="_blank">sklearn&#8217;s repository</a> and left all GAN code and hyper parameters untouched (which basically means that I rescaled the faces to have 28&#215;28 pixels dimension). The result is pretty similar:



It is fascinating how the G network converges (at probably 2/3 of the 2&#215;50&#8217;000 mini batches), and then basically varies lighting / shading / surrounding of a face, as well as mouth state (open/closed). But it can also be seen that some faces are severly damaged and look like from a zombie movie. While fuzziness of the pictures probably just has to do with the tiny size, the former phenomenon could do with some more experimentation in order to analyze the <a href="https://www.reddit.com/r/MachineLearning/comments/5fm66i/d_nips_2016_ask_a_workshop_anything_adversarial/" target="_blank">GAN training process</a>.

Some ideas for such further experiments (probably first on MNIST) could be to sample equidistant points from the z space and see how the generated images change when slightly modifying the z input; and how e.g. instances of the same digit are distributed in z space. This has already been done also for <a href="https://arxiv.org/abs/1606.05908" target="_blank">VAEs </a>and could give more intuition about the learned representation.

**Transfer to non-natural, non-pictorial images**

<span style="font-size: 1rem;">Neural networks that learn to generate content seem to be highly contageous &#8211; at least I unknowingly infected my graduate student Benj Meier with the idea, who conducted some experiments on his own (using a different code archive from the web). He trained the GAN to generate tumbnail pictures of newspaper pages on a dataset we got from the </span><a style="font-size: 1rem;" href="https://www.zhaw.ch/no_cache/en/research/personen-publikationen-projekte/detailansicht-projekt/projekt/2448/" target="_blank">PANOPTES project</a><span style="font-size: 1rem;">. The results are comparable to the abovementioned use cases, but here the images are ten times larger (256&#215;256, which is twice the size as the celebrated success on <a href="http://www.image-net.org/" target="_blank">ImageNet </a>by <a href="https://arxiv.org/abs/1606.03498" target="_blank">Salimans et al.</a>!):</span>



These preliminary experiments have been fun, but novel results and real use cases are still to be established. Meanwhile, the gained understanding will flow into our new <a href="https://www.msengineering.ch/en/home.html" target="_blank">MSE </a><a href="https://www.msengineering.ch/fileadmin/user_upload/customers/msengineering/Modulbeschreibungen/TSM_MachLe_en.pdf" target="_blank">lecture on machine learning</a>.

**A better training process? (update of Dec 01, 2016)**

Salimans et al.&#8217;s paper <a href="https://arxiv.org/abs/1606.03498" target="_blank">&#8220;Improved Techniques for Training GANs&#8221;</a> shows the potential of better insight into what is going wrong and how to remedy these errors; but watching the 2nd video above (synthesizing faces) gave me not only some intuition why GANs are considered hard/fragile to train, but also the following idea:

Usually, a mini batch for GAN training is comprised of m random images from the generator G(z), as well as m randomly drawn images from the training set for D(x). The G(z) and x values are thus unrelated, potentially leading to a situation where (say, for a dataset with images of fruits) the generator outputs apples, but the dataset (by chance) includes only oranges. Using this data to train, it teaches D to tell apples from oranges instead of fake from real, and G to paint oranges instead of more realistic apples (I exaggerate intentionally).

This lead me to the following potentially improved training process (experimental evaluation pending):

For the next mini batch, &#8230;

  1. Randomly draw m images from the training data
  2. For each x_i in the m images, let G generate a _visually fitting_ fake image by 
      1. Fixing G&#8217;s weights
      2. Optimizing the output G(z) (via gradient descent, by finding a suitable z) to best match the current x_i&#8230;
      3. &#8230;by e.g. <a href="https://arxiv.org/abs/1607.07539" target="_blank">minimizing the l1 norm between the pixel values</a> of both images.
  3. Proceed as usual by feeding D with the m training and m generated images, compute the usual loss and update D&#8217;s and G&#8217;s parameter according to the respective gradients

This way, the m generated images per mini batch are the best the generator can do in its current form to mimic this particular batch of training data. The discriminator should be able to learn subtle features much more quickly, and the generator could be driven to learn improve mimicking in general: instead of alternating _the kind of objects_ produced in each mini batch, it learns to improve _the appearance of objects_ themselves.

But so far, this is just an idea. Please let me know if you tried it out and have any insights!