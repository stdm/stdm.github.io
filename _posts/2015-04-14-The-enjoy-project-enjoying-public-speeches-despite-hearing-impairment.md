---
title: 'The ENJOY Project: Enjoying Public Speeches despite Hearing Impairment'
layout: post
categories:
  - Ethics
  - Research
---
During my spare time in the last year and ongoing, I have been involved in a very intersting project bringing together computer science expertise and charity: The ENJOY project (my term for it.

**Abstract.** Hearing-impaired attendants of large public events often find it impossible to follow speeches delivered via a loudspeaker/PA system even if they can follow normal conversations in small groups easily due to the aid of hearing implants. A possible remedy is simultaneous speech-to-text synthesis (speech recognition), so that the speech can be followed in reading live and on a private communication device like a tablet computer or smartphone.

Using the example of the public worship services of <a href="http://www.gvc-winterthur.ch" target="_blank">GvC Chile Hegi</a> in Winterthur, a team of four people has committed considerable resources since spring 2014 in researching and building a prototype of such a system.<!--more-->

### The Setting

The public worship services of GvC Chile Hegi are attended by approximately 800 people.  They consist of a mixture of live-played pop music and speeches (including e.g. announcements, interviews and a sermon) in a theatre-like setting. All performances are supported by certain media types in order for the people to get involved: Song lyrics are displayed in a multimedia show, speech is translated from Swiss German to several languages on wireless headphones for foreign visitors, and speakers are videotaped with a live playback streamed to a big central screen in order to be seen from every seat in the hall. However, if one is not able to follow what is said, most of the meaning is lost for this person.

In early 2014, a team of volunteers formed to help a hard of hearing / deaf attendee who desires to better follow the services. The team consists of a deaf person with a bone anchored and an ordinary hearing aid, a computer scientist having research experience in speech analysis, a closed caption author/translator with experience in re-speaking, and church leadership.

### Related Work

Besides manual sign language translation, one possible approach for helping hearing impaired persons enjoying public speeches is the application of speech recognition technology to auto-create some sort of closed captions for all speech parts during an event. Those closed captions could then be displayed either on the central video screen or streamed to personal communication devices (tablets, smartphones) of individual participants. Several approaches exist:

“<a href="http://www.mhsa.us/mhsa_cm.html" target="_blank">Caption Mic Classroom</a>” uses re-speaking of a speech to produce and stream live closed captions to personal devices. Due to <a href="http://www.mhsa.us/index.html#" target="_blank">diminishing demand</a>, the product is no longer sold or maintained. “<a href="http://www.cpcweb.com/brochures/youcaption_brochure.pdf" target="_blank">YouCaption</a>” has been a product with similar focus. It is no longer sold due to licensing issues and the companies’ customer service refers to <a href="http://www.nuance.com/index.htm" target="_blank">Nuance Communications Inc.</a> for possible alternatives. “<a href="http://successforkidswithhearingloss.com/interact-as" target="_blank">Interact-AS</a>” is a system for hearing-impaired pupils in classroom. It relies on specialized software on the laptops of pupils to deliver transcripts of what has been said.  A <a href="http://elearningbakery.com/lecture-capture-captioning-adobe-connect/#sthash.wE9sBEh0.dpbs" target="_blank">project conducted at the University of Leeds</a> in 2013 finally uses Dragon Naturally Speaking and a closed captioning tool from Adobe to build a system in assistance of deaf and hard-of-hearing students in translation studies.

As this brief review of the state of the art shows, there is no ready-made commercial system that supports the complete process from speech recognition to delivering the result end-to-end. But as the project in Leeds [8] demonstrates, it should be possible to build up this process using off-the-shelf components, uniquely orchestrated to fulfil the purpose of making public speeches enjoyable for hearing impaired persons. This view is also supported by several likewise reports [e.g., <a href="http://livecaptioningwithdragon.edublogs.org/" target="_blank">here</a>, and <a href="http://www.ngtvoice.com/services/assistive/transcription.htm" target="_blank">here</a>].

### Our Approach

Building on the results of this survey, the team decided to build a speech recognition based system out of available building blocks.

Current commercial speech recognition systems are capable of producing <a href="http://www.trustedreviews.com/nuance-dragon-naturallyspeaking-12-review-performance-and-issues-page-2" target="_blank">very accurate results</a>, given that their input is (a) free of interfering noises and of good linguistic quality and (b) the voice is known to the system via training. Systems are available for major languages; however, Swiss German dialect, which is mainly spoken at GvC, is currently not supported.

It has thus been decided to apply re-speaking to the original speech. It provides the best quality input to the system. A licence of Nuance’s Dragon Naturally Speaking 12 Premium has been acquired and trained to the professional re-speaker’s voice. (In the future, re-speaking could be possibly linked to the translation services for standard German language being available at GvC’s “Parkarena”, thus eliminating the need for any extra person being manually involved in generating the written text.)

Also, a dedicated workstation (dual Xeon X5570 with 8 cores, 18 GB RAM and SSD disc) has been acquired in late 2014 that is capable of a performant execution of the speech recognition software, allowing it to live-dictate into a <a href="https://docs.google.com/" target="_blank">Google Doc</a> via a web browser and <a href="http://www.nuance.com/extensions/index.htm" target="_blank">Nuance’s dictation plugin</a>. This allows for collaborative live editing of shared texts, thus by the way providing the sought live broadcasting feature.

The link to the Google Doc is shared among all participants of the pilot test and can be viewed on any private web-enabled device via GvC’s WLAN. In the tests, the Google Doc app for iPad has been used to follow a speech by reading. (In the future, the need for public Google Docs could be eliminated by setting up a private <a href="http://etherpad.org/" target="_blank">Etherpad server</a> with similar functionality.)

### Outlook

The prototype system works and is currently further evaluated before being integrated into GvC’s standard program for public worship services. Smaller issues are the display of the transcript (bright font on black background would be preferable in the darkened hall environment) and the used vocabulary (e.g., the German word for “bible” is usually confused with the word for “love”). Overall, the system is already capable to making the attendance of the services for hearing impaired people enjoyable by conveying the main message of speeches.

Nevertheless, medium- to long-term goals remain:

  * Productizing the prototype for a better, easier-to-use experience for all involved persons: 
      * Having a specialized app that just displays the transcript of the current speech
      * Training the speech recognizer with old speech manuscripts for appropriate vocabulary
      * Better integration of the different tools currently used in the process
  * Optimizing speech recognition for live transcription settings 
      * Coping with dictation tempo
      * Dealing with a more standard speaking style (to be able to receive input from any major language translator, not just explicit re-speakers)