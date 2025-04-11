---
title: How not to fear AI? 
layout: post
date: 2025-04-11
modified: 2025-04-11
category: AI, society, hope, risk, fear, TESCREAL, talk
comments: true
---

Circa two years ago, I started investigating, and putting into words and talks, how a technically grounded understanding of AI can help mitigate unwarranted fears. [KCF 2023](https://www.youtube.com/watch?v=0Sk_mX0dSCQ) in Berlin was a kick-off, after which many requests reached me to extend this material and make it available to larger audiences. May sabbatical added depth (see [here](https://stdm.github.io/Risk/), [here](https://stdm.github.io/Hope/), and [here](https://stdm.github.io/AI-sports-humanism/)). When Tilman Slembeck asked in January if I wanted to join TEDxZHAW "Merging Worlds" as a speaker, I felt ready. 

<!-- more -->

Little did I know how much preparation still awaited me. I easily invested more than one order of magnitude more effort here than in any other talk I ever prepared. As the TED format asks for a different style than I usually do (shorter, story-focussed, less slides, speaker-centered), I had to change my whole approach to creating and then practicing a talk. I felt like a boxer who had prepared intensely for months for this one fight: I created 12 iterations of slides; wrote a script for the talk for the first time in my life; rehearsed and updated it every free minute for the last two weeks; gave premature versions of the talk to my colleagues at least once a day. Thanks to this preparation, we now have a full script of the talk available. I want to share it with you below (video will come soon).

![TEDx preparation](http://stdm.github.io/images/TEDx/tedx-prep.jpg)

It is 1997. Chess world champion Garri Kasparov takes on Deep Blue - the most advanced chess AI system of its time. High noon for human versus machine. Then it happens, already in the first game: Kasparov observes an AI move that he cannot understand. 

This move is pure randomness, the result of a bug in Deep Blue's software. But instead of realising the machine's limitations, Kasparov is overtaken by fear: He thinks this move is a sign of higher intelligence, and concludes that the machine might be unconquerable with his mere human strategies [^1]. That throws him off track with his match plan - and ultimately, he loses. Kasparovs defeat became known as the first big loss of humankind against AI. But **the human lost not because of the machine's abilities but because of the man's fears**.

Today, I observe something similar: In my capacity as a professor of AI, I get to discuss AI with a lot of different people. And one topic keeps surfacing: people's fear of AI. They share their concerns of being displaced in their job by a future chat bot; of becoming so dependent on some system to lose critical skills for mastering their life independently; of losing their very life to an AI overlord turning against them.

How warranted are such fears? Or: How sober can we afford to think about one of the most defining trends of our times? I would like to help you answer that question based on a clear understanding of what AI is and isn't and where some of the most intimidating ideas on this topic come from. 

So what is AI? It has been defined as the **simulation of intelligent behaviour with a computer** [^2]. AI thus is not about the creation of intelligent beings. It is about mimicking the result of intelligence - by any means available, a whole toolbox full actually, dependent on the intended behaviour. Arguably, the most prominent means of AI in the last 2 decades has been "machine learning". We use machine learning if the behaviour we want to simulate cannot be described by a set of rules.

![TEDx cats & dogs example](http://stdm.github.io/images/TEDx/tedx-catsdogs.jpg)

Consider classifying a set of images into the categories "cats" and "dogs". We cannot find a set of rules - but give a set of examples of input to the system (visual features of images) and corresponding output (the category). They can be separated by a function relating input to output. Learning then means to systematically manipulate the parameters of that function to fit the given examples. This is done with a mathematical device we all learned about in school: the chain rule of differentiation.

So what does this function actually implement?

![TEDx functional form images](http://stdm.github.io/images/TEDx/tedx-pimages.jpg)


The probability (*p*) of the category (*y*) given the visual features (*x1*, *x2*).

Now, machine learning works not only with simple visual features and straight lines. We can put in all the pixels of the images. Then use a more wiggly function template called a "neural net" [^3]. And then scale to more data to learn a more nuanced relationship. 

It also works with other input-output pairs, e.g. text as input and its likely continuation as output. This gives us "large language models" - the engine behind products like ChatGPT and the arguable pinnacle of modern AI. A LLM then models the following relationship: 

![TEDx functional form LLM](http://stdm.github.io/images/TEDx/tedx-ptext.jpg)

Quite familiar, the probability (*p*) of the next token (or sub-word) (*y*) given the previous tokens in the context window of size *C*.

Quantitatively, this context can become as large as millions of words. The respective function will have billions of parameters to fit such data well. And it needs a full internet of text to be well trained.

What can we say qualitatively about such a model?
 
Well, it is a statistical model. That differentiates it quite drastically from how humans work. For example, **a statistical model has no concept of truth and facts** - it has just learned about statistical plausibility. On average, this will be very useful and even outperform humans. But: In any individual case, it may be wrong, because of the fundamental limitation of no facts and truth, just coincidences and correlation instead of causation.

Let's make this concrete: I asked one of the leading so-called "reasoning" models the following question:

> The surgeon, who is the boy's father, says "I can't operate on this boy, he is my son!" Who is the surgeon to the boy?"

The answer should be straight-forward and is even contained in the text: "Who is the boy's father". Now the model computes for 10 seconds and replies:

> "The surgeon is the boy's mother."

Which if profoundly stupid. But to the model, this makes actually sense - and it tells us why: 

> "The riddle plays on the assumption that a surgeon is male"

it tells us. And actually, variations of my question exist in abundance on the web as tests for our own human biases: Namely our gender bias that usually associates males with the role of a surgeon. So the model has seen all these during its training and learned the utter statistical implausibility of answering anything male to a question that looks remotely like mine.

So the model's answer is plainly wrong - and totally plausible for any AI system build according to the principles of machine learning at scale. Unfortunately, we don't' have other principles. Not now and not at the horizon of research. So **fundamental limitations like this - while examples come and go - will stay with us** also with GPT 5, 6, 7 et cetera. 

How does this compare to the human? [^4]

We said AI simulates intelligent behaviour. And we saw it does so by completely different means than human intelligence. These means have fundamental limitations - we just saw one example, the lack of veracity, there are many more. 

These **different means constitute a difference *in kind* to human nature**. Think of it using the analogy of a musician and a DJ: While a DJ simulates certain aspects of creating music very well, their method of music creation by design is not general. There are so many aspects of music beyond the method of turntables and remixing. Certain genres. Certain techniques. Certain settings. Similarly, **AI does *not* simulate humans, but certain carefully designed aspects of human behaviour, with a very specific method of cleverly interpolating between pre-recorded behaviour samples**.

What then is **the future of such AI? It is *not* Artificial General Intelligence**, whatever this means precisely. It is not an "AI overlord"" on eye level with humanity. 

![TEDx computer control](http://stdm.github.io/images/TEDx/tedx-computercontrol.jpg)

But likely quite helpful personal assistants able for example to operate our computer to do our bidding [^5]. Still limited by imperfections, but useful.

Where, then, does this fear of AI come from?

![TEDx fear](http://stdm.github.io/images/TEDx/tedx-fear.jpg)

It does not have a strong basis in the technology we have, or in the underlying science we just saw. **Here is the thing: Such fear is rather based on wide-spread narratives**. And these dystopian narratives are purely based on world view - on science fiction, not on tech. 

Let me explain. AI ethicists Timnit Gebru and Emile Torres recently analysed the respective world views, and coined the acronym TESCREAL to refer to Transhumanism, Extropianism, Singularitarism, Cosmism, Rationalism, et cetera [^6]. They show how respective philosophies are widespread in the tech industry, and how they profoundly shape the global narratives on AI. You find traits of TESCREAL in movies like "The Matrix", or in the books of Prof. Harari. In fact, they have become the mainstream school of thought in Silicon Valley [^7]. See for example the 2023 "Open Letter" on an AI research moratorium to circumvent existential risk. It was, as co-originator Prof. Max Tegmark of MIT is very open to explain at length in a podcast [^8], purely based world view, not on a single technical argument. 

Instead, the TESCREAL narrative for AI goes like this: Humans are nothing but information processors - just on biological, decaying hardware. This makes them akin to machines, just inferior, because of the fragile hardware (that's the Rationalism above). If humans could gain intelligence, then nothing prevents machines from reaching the same. Soon. And this intelligence will just increase ever further to AGI and beyond (that's the Singularitarism). So humans should upgrade themselves to become more like machines (that's the Transhumanism). It goes without saying that this view is highly contested from different scientific disciplines.

Summarizing, the TESCREAL philosophies are characterized by having little regard for human worth and dignity. It comes at no surprise that they exaggerate machine competence and make people feel small, intimidated and worthless. But this is philosophy, not inevitable science. If TESCREAL is not your world view, there is considerably less to fear about AI.

![TEDx sunrise](http://stdm.github.io/images/TEDx/tedx-sunrise.jpg)

So how not to fear AI? It begins with the realisation that **the AI you fear does not exist**. AI is a tool. If that helps, rename AI to  "EI" - Extended Intelligence, as we have recently argued in an article [^9]. Because extending our own human capabilities is all AI can do: Help us to improve our lives. Not replace us. So an insurmountable categorical difference remains: Agency ultimately stays with us, for the better or worse. 

This means that AI is *not* coming after your freedom nor anything in your life. That is good news. But you might lose your freedom to AI in a different way - by giving it up voluntarily! We need to look at how this can happen:

First, **we might surrender our freedom prematurely to non-existent machine competence**. Like this: 

> Oh AGI, you calculate probabilities precisely and store so many patterns -
> What shall I eat today?
> What vocation shall I train for?
> Whom shall I marry?
> Shall I marry at all?

Don't laugh - this happened before in the history of human-AI relationship: Remember Kasparov vs. Deep Blue from the beginning? Kasparov didn't primarily lose against an excellent chess computer. First and foremost, he lost the battle in his mind against his assumption of an unconquerable AI. 

Second, **we might become defenceless against the endless conveniences that AI tools offer**, and hence fail to become the person we ought to be. It is part of our human nature that we need to learn, mature, grow. And all growth includes an element of pain - think of sports. If we forego too many opportunities for growth by for example letting AI write the essay, solve the task, enquire the information, we might forfeit future freedom by not forming the character and skills necessary to wield such powerful tools.

Fortunately, there is a mitigation strategy against these only two ways how you can loose to AI: **Know you worth and dignity as a human being!** If you can say with the parents of the universal declaration of human rights: 

> I am wonderfully made. I have purpose. I love and am loved. I thrive on human relationships. I am endowed with exceptional skills, but I am more than my skillset.

Then you feel not intimidated by a powerful tool. You don't surrender to it. You treat yourself, even with necessary pain for growth.

We are almost there. But... aren't there real risks of AI, philosophy or not? Yes, absolutely. 

Here is one typical list of AI risks, from the many similar ones that exist in the literature [^10]. But equipped with the arguments we just discussed, on the nature of the technology and surrounding narratives, this list splits into two list:

![TEDx risks](http://stdm.github.io/images/TEDx/tedx-risks.jpg)

On the right, many of the points that make people fear AI. Now, they appear exaggerated - like the fear of major job displacements. Because AI tools can automated tasks, but cannot automate the whole you. And controllable - like your own dependence on these tools. And, finally, purely hypothetical - like the existential risk of rogue AI overlords exterminating humanity.

What is left, are the risks in green. Existent, real. But these challenges are manageable: Some technologically, some socially, some regulatory. Approaches exist, literature and practice are full of them [^11]. 
Its not all solved yet. But we can handle this.

So that's how not to fear AI:

1. **Consider it as Extended Intelligence**. It is a tool, built on probability functions, and has fundamental limitations. Don't overestimate its scope.
2. **Reject fears purely based on a world view that you probably don't share** and that is rooted in a view of humanity and of technology that comes from science fiction, and not from reality.

Instead, **contribute to creating the future you want to live in. Use AI where appropriate. Tools are for the worker** [^12].

Enjoy.

[^1] Silver (2012), "The signal and the noise: Why so many predictions fail - but some don't". Penguin Press, ISBN 978-1594204111. (Relating the story of Kasparov vs. Deep Blue in Chapter 9.)
[^2] Stadelmann (2025), ["A guide to AI: Understanding the technology, applying it successfully, and shaping a positive future"](https://www.globalresiliencepub.com/wp-content/uploads/2025/01/Global-Resilience-White-Paper-2-A-GUIDE-TO-AI-by-Dr.-Thilo-Stadelmann.pdf). Global Resilience White Papers No. 2. 
[^3] Prince (2023), ["Understanding deep learning"](https://udlbook.github.io/udlbook/). The MIT Press, ISBN 978-0262048644.
[^4] Lawrence (2024), "The atomic human". Allen Lane, ISBN 978-0241625248.
[^5] Sager et al. (2025), ["AI agents for computer use: A review of instruction-based computer control, GUI automation, and operator assistants"](https://arxiv.org/abs/2501.16150). ArXiv preprint 2503.01411.
[^6] Gebru & Torres (2024), ["The TESCREAL bundle: Eugenics and the promise of utopia through artificial general intelligence"](https://firstmonday.org/ojs/index.php/fm/article/view/13636). First Monday 29(4).
[^7] Torres (2023), ["The acronym behind our wildest AI dreams and nightmares"](https://www.truthdig.com/articles/the-acronym-behind-our-wildest-ai-dreams-and-nightmares/). Truthdig, June 15.
[^8] Fridman (2023), ["Max Tegmark: The case for halting AI development"](https://www.youtube.com/watch?v=VcVfceTsD0A). Lex Fridman Podcast #371.
[^9] Segessenmann et al. (2023), ["Assessing deep learning: A work program for the humanities in the age of artificial intelligence"](https://link.springer.com/article/10.1007/s43681-023-00408-z). AI and Ethics 5, 1-32.
[^10] Jackson (2024), ["Top 10: Risks of AI"](https://aimagazine.com/top10/top-10-risks-of-ai). AI Magazine, August 21.
[^11] Wehrli et al. (2021), ["Bias, awareness and ignorance in deep-learning-based face recognition"](https://link.springer.com/article/10.1007/s43681-021-00108-6). AI and Ethics 2, 509-522. (An example of a mitigation strategy for a manageable AI risk - bias.)
[^12] Davison (2024). ["Tools are for the worker"](https://www.mohrsiebeck.com/artikel/tools-are-for-the-worker-101628ptsc-2024-0014/). Philosophy, Theology and the Sciences 11(2).
