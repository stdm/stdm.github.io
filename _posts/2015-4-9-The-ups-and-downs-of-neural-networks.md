---
title: The ups and downs of Neural Networks
layout: post
guid: https://dublin.zhaw.ch/~stdm/?p=241
categories:
  - Readings
  - Research
tags:
  - current research
  - Deep Learning
  - history
---
Interesting enough, the current hype topic (rightly so!) in Machine Learning is Deep Learning &#8211; which is largely the current term for ongoing research in Neural Networks.

## Why is this interesting?

Neural Networks have a colourful history. Being researched first in the 1950&#8242;s as biologically inspired machine learning approaches (though that term wasn&#8217;t used then), they repeatedly

  * excited the fanasies of users and laypeople,
  * stirred and subsequently disappointed the exaggerated expectations,
  * fell out of favour as if &#8220;we tried that; it didn&#8217;t work&#8221;,
  * just to rise again as new results showed superiority compared with other approaches on previously unseen tasks.<!--more-->

<div id="attachment_242" class="wp-caption alignnone" style="width: 635px">
  <a href="http://stdm.github.io/images/NN-History.jpg"><img class="size-large wp-image-242" title="Neural Network hisotry in writing." alt="NN-History" src="http://stdm.github.io/images/NN-History.jpg" width="625" height="305" /></a>
  
  <p class="wp-caption-text">
    Three famous NN publications: Minsky&#8217;s &#8220;Perceptrons&#8221;, Rumelhart&#8217;s &#8220;Parallel Distributed Processing&#8221; and LeCun&#8217;s &#8220;Gradient-based Learning Applied to Document Recognition&#8221;.
  </p>
</div>

This up and down is readily observed in the literature (see the picture): Inflated expectations in the 1950&#8242;s and 1960&#8242;s where shattered by (largely a misunderstanding of) Minsky et al&#8217;s &#8220;Perceptrons&#8221; of 1969, which lead to the first so-called <a href="http://en.wikipedia.org/wiki/AI_winter" target="_blank">&#8220;AI winter&#8221;</a>. Rumelhart et al&#8217;s &#8220;Parallel Distributed Processing&#8221; from 1987 swung the pendulum to the other side again with new results and ideas. These where again not directly transferable to all applications domains, leading to another AI winter in the 1990&#8242;s.

In 2006, <a href="http://www.cs.toronto.edu/~hinton/absps/ncfast.pdf" target="_blank">Hinton et al</a> finally showed how to train deeper architectures of Neural Networks and thus realize their full potential. This kicked off a whole bunch of new and continued dedicated &#8220;Deep Learning&#8221; (a.k.a. Representation Learning) research that culminated an most of all pattern recognition benchmarks won by a large margin through deep learning approaches within the last 4 years &#8211; see Schmidhuber&#8217;s excellent survey of the history of Deep Learning research and achievements <a href="http://arxiv.org/abs/1404.7828" target="_blank">here</a>.

<div id="attachment_243" class="wp-caption alignnone" style="width: 471px">
  <a href="http://stdm.github.io/images/lecun-hinton-bengio-schmidhuber.jpg"><img class="size-full wp-image-243 " title="Big 4 in DL" alt="lecun-hinton-bengio-schmidhuber" src="http://stdm.github.io/images/lecun-hinton-bengio-schmidhuber.jpg" width="461" height="127" /></a>
  
  <p class="wp-caption-text">
    Big Names in Deep Learning (left to right): Yann LeCun, Geoffrey Hinton, Yoshua Bengio and Juergen Schmidhuber.
  </p>
</div>

As an interesting side note, the heads of what are on my perception the top 4 research groups in Deep Learning world wide are the one that already helped to shape the field since the 1980 (compare the second picture): Geoffrey hinto for example was already a coauthor in Rumelhart et al&#8217;s work on Parallel Distributed Processing. Yann LeCun and Yoshua Bengio wrote <a href="http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf" target="_blank">an articel</a> in 1998 that is still foundational to the mastering of Convolutional Neural Nets (a.k.a. ConvNets), a recently very fashionable approach even besides image processing. According to Jonathan Masci&#8217;s <a href="http://www.s-i.ch/fileadmin/daten/sgaico/keynote_masci_small.zip" target="_blank">Keynote</a> at last year&#8217;s &#8220;Intelligent Systems and Applications&#8221; conference, most that changed since then are small algorithmic adjustments to facilitate the training of deeper architectures and huge improvements in hardware power (via GPUs mainly).

## What are we going to do about it?

The <a href="http://www.zhaw.ch/datalab" target="_blank">Datalab </a>invested considerably in <a href="http://www.zhaw.ch/de/zhaw/institute-zentren/uebergreifende-institute-zentren/dlab/hardware.html" target="_blank">parallel computing hardware</a> last year in order to kick off Deep Learning research at ZHAW. A group of about 10 researchers formed, reading foundations and gaining momentum by implementing prototypes for various applications including face recognition and OCR. First projects are already finished, and more are yet to come.