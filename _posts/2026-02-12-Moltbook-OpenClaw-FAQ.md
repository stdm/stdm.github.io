---
title: The Moltbook and OpenClaw FAQ
layout: post
date: 2026-02-12
modified: 2026-02-12
category: AI, society, agents, narratives, AGI
comments: true
---

[Moltbook](https://www.moltbook.com/) and [OpenClaw](https://openclaw.ai/) agents still seem to be the talk of the town after going viral in January 2026. Time for a few brief answers to the frequently asked questions (thanks to Nicolas Eggen of [Nau media AG](https://www.nau.ch/) for providing the questions). So here it is: The "hot to stay sane" Moltbook/OpenClaw FAQ.


![Moltbook FAQ](http://stdm.github.io/images/moltbook-faq.png)

<!-- more -->


#### What is the purpose of Moltbook - what is it meant to achieve? Is it just entertainment for people? What concrete goals are the initiators pursuing?

It is a fun project that went viral. That also makes it a large-scale experiment from which something useful might eventually emerge (in many years, once such agents become secure and therefore practically usable). If machine agents are someday equipped with certain autonomy to carry out tasks for us, an 'exchange' among them about best practices might make sense. But at the moment, this is a playground, and we should be careful not to read too much into it.

#### To what extent are the interactions between the agents actually autonomous versus initiated, controlled, or influenced by humans? Expert reports suggest that many bots are under human control and that their autonomy is overestimated. So is Moltbook ultimately just hot air - are humans the ones pulling the strings behind the scenes?

I have read similar reports but have no further information beyond that. My assumption would be that, quantitatively, most of them are bots; however, particularly in the case of the biggest 'outrages,' I would be skeptical about whether a human agitator might be behind them. See above: a lot of fun, a large playground, a huge, uncontrolled experiment. Do not overinterpret it (neither on the level of content nor on the structural level).

#### How realistic is it to interpret certain content (e.g., philosophical or 'revolutionary' statements) as signs of independent AI intelligence? E.g., Elon Musk has described Moltbook on his platform X as a harbinger of the singularity - the point at which AI surpasses humans. Do you share this assessment?

That is nonsense. LLMs - the type of AI models behind the OpenClaw bots - are, by their nature, high-dimensional probability density functions that infer the most likely next token (think: word) from a sequence of token (words) [^1]. They were trained on virtually all text on the internet, including vast amounts of sci-fi pulp fiction in which AI takes over the world, gains consciousness, etc. On Moltbook, these probability density functions are now sampling each other within a context that (via pre-prompts, etc.) ascribes 'autonomy' to them. Of course the result is what we are reading; that is not surprising in the slightest and is most easily explained by these statistical phenomena [^2]. At the same time, initial studies show that threads on Moltbook are highly redundant (30-40% textual overlap, compared to much less among humans [^3]). This, too, strongly suggests that beyond the sampling process there is nothing deeper to discover (unless one is inclined to see it that way based on one's worldview, which is an important and never to be undererstimated driver of AI opinion [^4]).

#### What security and data protection risks are known in connection with Moltbook or the underlying agent system? What dangers do you see in terms of misuse (e.g., spam, data theft, automated attacks)?

Without going into detail: OpenClaw bots are a security disaster for their users. That is precisely one of the reasons why I wrote above that real applications of such agents may still be years away. It is a massive engineering challenge (as well as a legal, regulatory, and societal one) to make these early prototypes truly suitable for everyday use [^5]. This includes security, but also the fact that LLMs inherently make constant errors, which will not disappear quickly due to their underlying design principles [^6].

#### What distinguishes the media hype narrative (e.g., AI bots developing an 'own society') from the technical reality? How should the public assess such 'experiments' in a sober manner? Which expectations are realistic, and which are exaggerated?

Much of this has already been said above. The narratives about an 'own society,' consciousness, etc. are deliberately spread by highly influential opinion leaders because it is good for business (see the hype around so-called 'AGI'). Technically, there is not a single valid argument supporting such claims [^7]. 


## Footnotes

[^1]: See ["The sotchastic nature of machine leanring"](https://stdm.github.io/downloads/papers/AIEthics_2026.pdf) for a deeper, still readable, explanation.
[^2]: There is a core principle in the otherwise not very principle-rich discipline of machine learning, 'Occam's Razor': if two explanations explain a phenomenon equally well, go with the simpler one (and reject the more complex one). We don't need to summon machine consicousness and AGI to explain Moltbook. PDFs sampling themselves is sufficient.
[^3]: Compare Ethan Mollick's pleasently calm [post](https://www.linkedin.com/posts/emollick_if-you-have-been-paying-attention-to-the-activity-7423254129172631552-wrRQ/).
[^4]: See the intro in ["Evidence-based AI risk assessment for public policy"](https://www.tandfonline.com/doi/full/10.1080/09540962.2025.2541304) for an explanation of the relationship of worldview and AI predictions.
[^5]: Cp. ["A comprehensive survey of AI agents for computer use"](https://arxiv.org/abs/2501.16150) and Simon Willis' very readable [post](https://simonwillison.net/2026/Jan/30/moltbook/) for some background on the technical challenges alone.
[^6]: I've expanded on this topic in my TEDx talk ["How not to fear AI"](https://youtu.be/deVbP-hViMQ) and the ["Guide to AI"](https://www.globalresiliencepub.com/wp-content/uploads/2025/01/Global-Resilience-White-Paper-2-A-GUIDE-TO-AI-by-Dr.-Thilo-Stadelmann.pdf).
[^7]: An overview is given in the TEDx talk ["How not to fear AI"](https://youtu.be/deVbP-hViMQ); further strong arguments are provided by Arvind Narayanan and Sayash Kapoor on their [blog](https://www.normaltech.ai/) and the corresponding article ["AI as normal technology"](https://knightcolumbia.org/content/ai-as-normal-technology).