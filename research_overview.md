---
title: Research
layout: page
comments: false
---

The Machine Perception and Cognition group occupies a distinctive position at the intersection of applied and foundational AI research. It is firmly motivated by practical problems (ca. 80% of our research is joint work with practice partners), yet consistently engages fundamental questions about, e.g., what data science <em>is</em>, how natural intelligence works, and what ML's stochastic nature means for safety, publishing  at top venues regularly (ICML, Nature Scientific Reports, Pattern Recognition, AI and Ethics etc.). Below is a summary of some defining traits that emerge consistently across the full publication record of >100 papers from >20 years, geasred towards researchers.

### TOC
1. [The mindset behind our work](#mindset)
2. [Research lines](#research)
3. [Examples of translation into practice](#practice)
4. [Main scientific contributions](#contributions)


<img alt="Thilo Stadelmann and Yann LeCun discussing world models and cowbell blues at the Swiss AI Award 2023 ceremony in Davos, Switzerland" src="http://stdm.github.io/images/stdm-lecun.jpg"/>


<a name="mindset"></a>
## The mindset behind our work

<div style="background:#f0f5fb; border:1px solid #bdd0e8; border-radius:6px; padding:20px 26px 14px; margin:1.2em 0 2em;">


<div style="display:grid; grid-template-columns:repeat(auto-fill, minmax(300px, 1fr)); gap:14px; margin-top:1em;">

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Principled pragmatism.</strong> Problems must matter outside the lab, but engineering alone is not enough. There is a recurring impulse to step back and ask "what general principle explains this?", leading to design-pattern taxonomies, the data-centrism argument, a theory of natural intelligence, or the ATLAS teaching concept.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Translator instinct.</strong> A substantial share of the output (e.g., the Applied Data Science book (with &gt;123 k readers), "Deep Learning in the Wild," or white papers for policymakers) explicitly closes the gap between what researchers know and what practitioners and regulators can act on.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Emoirical honesty.</strong> Several of the strongest papers report negative or counter-intuitive findings: DNNs for speaker recognition don't learn temporal voice features; blinding face-recognition models to sensitive attributes doesn't reduce demographic bias; ImageNet-optimal architectures don't transfer across domains.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Disciplinary self-consciousness.</strong> Unusual for a technical ML group, we invest sustained effort in defining what our own discipline fundamentally <em>is</em>. The data-centrism paper, the ECSS and HMD series, or the "Foundations of Data Science" overview are acts of disciplinary self-definition.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Long arcs alongside rapid response.</strong> Some threads run for more than a decade (speaker recognition, optical music recognition, applied data science). Others respond quickly to emerging topics (LLM efficiency, AI agents survey, stochasticity and safety). A stable intellectual core with enough flexibility to engage new problems without losing continuity.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Genuinely interdisciplinary collaborators.</strong> Co-authors span radiologists, physicists, geothermal engineers, cognitive neuroscientists, musicologists, social workers, transport engineers, and ethicists. Domain knowledge visibly shapes methodology in each case.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Applied science identity, worn lightly.</strong> The Fachhochschule mandate (problems must be real) is treated as the motivational inspiration rather than a ceiling on ambition. ICML papers and Neural Computation articles coexist with industrial reports and practitioner handbooks.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Education as a research topic.</strong> Teaching AI is treated as an object of scholarly inquiry, not just a duty. The ATLAS concept, the EducSci paper on hybrid AI education, and the Bürgenstock higher education workshop reflect a conviction that how we teach shapes what the field becomes.
</div>

</div><!-- trait grid -->
</div><!-- character box -->


<a name="research"></a>
## Research lines

Being motivated by real-world pattern recognition problems (how perceptions are formed from sensory input and cognitively tranlated into reasonable actions) leads to a suprinsingly broad field of use cases and industries amidst a stable core of methodological focal points. Here's an overview of sub-disciplines our inquiry contributes to.


<br>

<details markdown="1">
<summary><b>Speaker recognition & audio representation learning</b></summary>

*~2004–ongoing: formative line from PhD to continued breakthroughs with deep learning*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465"><img src="http://stdm.github.io/images/papers/PhdThesis_2010.jpg" alt="PhD Thesis 2010" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ICASSP_2006.pdf"><img src="http://stdm.github.io/images/papers/ICASSP_2006.jpg" alt="ICASSP 2006" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3761"><img src="http://stdm.github.io/images/papers/MLSP_2016.jpg" alt="MLSP 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3762"><img src="http://stdm.github.io/images/papers/MLSP_2017.jpg" alt="MLSP 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patrec.2024.03.016"><img src="http://stdm.github.io/images/papers/PRL_2024a.jpg" alt="PRL 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

The earliest sustained research thread centres on automatic speaker recognition. The [PhD thesis](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) (Marburg, 2010) introduced the *Dimension-Decoupled Gaussian Mixture Model* for coping with very short speech segments and established that improved recognition hinges at exploting temporal cues in a voice. Later work introduced deep learning to the field: CNNs applied directly to spectrograms ([MLSP'16](https://doi.org/10.21256/zhaw-3761), >100 citations) proved competitive for both speaker identification and clustering. Subsequent work used RNNs to capture supra-segmental voice characteristics ([ANNPR'18b](https://doi.org/10.1007/978-3-319-99978-4)) and metric-learning embeddings for measuring voice similarity ([MLSP'17](https://doi.org/10.21256/zhaw-3762)). A 2024 *Pattern Recognition Letters* paper delivers a sobering counter-result: deep networks for speaker recognition [*do not yet learn supra-segmental temporal features*](https://doi.org/10.1016/j.patrec.2024.03.016), raising open questions about what these models actually learn.

| Paper | Key finding / message |
|---|---|
| [Stadelmann, PhD thesis (2010)](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) | Supra-segmental temporal features are key to unlocking an order of magnitude lower error rates. |
| [Lukic et al., MLSP'16](https://doi.org/10.21256/zhaw-3761) (>100 citations) | CNN on spectrograms achieve state-of-the-art speaker ID and clustering without hand-crafted features. |
| [Stadelmann et al., ANNPR'18b](https://doi.org/10.1007/978-3-319-99978-4) | RNNs seem to capture supra-segmental prosodic features for improved voice clustering. |
| [Neururer et al., PRL 2024](https://doi.org/10.1016/j.patrec.2024.03.016) | DNNs for ASR learn spectral but *not* temporal features, even if they could: the models are more superficial than expected. |
</details>

<details markdown="1">
<summary><b>Applied deep learning: from benchmarks to production</b></summary>
*~2016–ongoing: Centrepiece applied-ML research programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.1007/978-3-319-99978-4"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" alt="DL in the Wild" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/SDS_2019.pdf"><img src="http://stdm.github.io/images/papers/SDS_2019.jpg" alt="SDS 2019" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://www.mdpi.com/2673-2688/1/4/31"><img src="http://stdm.github.io/images/papers/AI_2020.jpg" alt="AI 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/TAILOR_2020.pdf"><img src="http://stdm.github.io/images/papers/TAILOR_2020.jpg" alt="TAILOR 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3389/fcomp.2022.1041703"><img src="http://stdm.github.io/images/papers/Frontiers_2022.jpg" alt="Frontiers 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A distinctive contribution is the systematic study of the gap between benchmark-driven research and real-world deployment. The invited paper [*"Deep Learning in the Wild"*](https://doi.org/10.1007/978-3-319-99978-4) (ANNPR'18) distils lessons from six production use cases. The companion book chapter [*"Beyond ImageNet"*](https://stdm.github.io/downloads/papers/ADS_2019_DeepLearning.pdf) (Springer, 2019) generalises these into transferable principles. The MDPI AI paper on ["Design Patterns for Resource-Constrained Automated Deep-Learning Methods"](https://www.mdpi.com/2673-2688/1/4/31) (2020) synthesises the methodological takeaways into reusable patterns. The [Frontiers'22 paper](https://doi.org/10.3389/fcomp.2022.1041703) closes the loop empirically, showing that ImageNet-optimal architectures fail to transfer across domains.

| Paper | Key finding / message |
|---|---|
| [Stadelmann et al., ANNPR'18d](https://doi.org/10.1007/978-3-319-99978-4) | Real deployment requires wrapping core DL models in ensembles of auxiliary modules; benchmark accuracy is necessary but not sufficient. |
| [Stadelmann et al., ADS ch. *Beyond ImageNet* (2019)](https://stdm.github.io/downloads/papers/ADS_2019_DeepLearning.pdf) | Most industrial DL projects require domain-specific data curation, loss shaping, and calibration absent from canonical ImageNet training. |
| [Tuggener et al., MDPI AI 2020 *Design Patterns*](https://www.mdpi.com/2673-2688/1/4/31) | Seven reusable design patterns cover the majority of resource-constrained AutoML scenarios. |
| [Tuggener et al., Frontiers 2022](https://doi.org/10.3389/fcomp.2022.1041703) | CNN architectures optimised on ImageNet do not reliably transfer across domains, hence architecture search must be domain-aware. |
</details>


<details markdown="1">
<summary><b>Data Science as a scientific discipline</b></summary>
*~2013–2022: conceptual / disciplinary foundation work*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://stdm.github.io/downloads/papers/ECSS_2013.pdf"><img src="http://stdm.github.io/images/papers/ECSS_2013.jpg" alt="ECSS 2013" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3759"><img src="http://stdm.github.io/images/papers/HMD_2014.jpg" alt="HMD 2014" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/978-3-658-11589-0_4"><img src="http://stdm.github.io/images/papers/HMD_2016.jpg" alt="HMD 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/data-science-book/"><img src="http://stdm.github.io/images/papers/ADS_2019.jpg" alt="ADS book 2019" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ADS_2019_DataScience.pdf"><img src="http://stdm.github.io/images/papers/ADS_2019_DataScience.jpg" alt="What is Data Science" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

Running parallel to empirical research is a sustained effort to define and legitimise *data science as a discipline in its own right*. The early papers ([ECSS'13](https://stdm.github.io/downloads/papers/ECSS_2013.pdf), [HMD'14](https://doi.org/10.21256/zhaw-3759), [HMD'16](https://doi.org/10.1007/978-3-658-11589-0_4)) characterised the emerging role of the "data scientist." The Springer edited volume [*Applied Data Science*](https://stdm.github.io/data-science-book/) (2019, >123 000 accesses) became a widely-read practitioner reference. The 2022 *Archives of Data Science* paper [*"Data Centrism and the Core of Data Science"*](https://dx.doi.org/10.5445/IR/1000143637) provides the most theoretically developed argument: that *data centrism*, treating data as the central object of study rather than a means to an end, is the overarching principle distinguishing data science from statistics, ML, and data management.

| Paper | Key finding / message |
|---|---|
| [ECSS'13](https://stdm.github.io/downloads/papers/ECSS_2013.pdf); [HMD'14](https://doi.org/10.21256/zhaw-3759); [HMD'16](https://doi.org/10.1007/978-3-658-11589-0_4) | The data scientist profession requires a unique combination of analytics, technology, entrepreneurship, and communication; none of the contributing disciplines provides this alone. |
| [Braschler, Stadelmann, Stockinger (Eds.), Springer 2019](https://stdm.github.io/data-science-book/) (>123k accesses) | 16 case-study chapters; central lesson: "necessity is the mother of invention" - applied data science is always problem-driven, not method-driven. |
| [Stadelmann, Klamt, Merkt, AoDSA'22](https://dx.doi.org/10.5445/IR/1000143637) | *Data centrism* (data as the central subject, not a resource) is the unique disciplinary core that no contributing field shares to the same degree. |
</details>


<details markdown="1">
<summary><b>Document recognition & optical music recognition</b></summary>
*~2017–ongoing: dedicated dataset and methods programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" alt="ICDAR 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-4255"><img src="http://stdm.github.io/images/papers/ICPR_2018a.jpg" alt="ICPR 2018a" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3760"><img src="http://stdm.github.io/images/papers/ISMIR_2018.jpg" alt="ISMIR 2018" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/WoRMS_2018.pdf"><img src="http://stdm.github.io/images/papers/WoRMS_2018.jpg" alt="WoRMS 2018" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ICPR_2020.pdf"><img src="http://stdm.github.io/images/papers/ICPR_2020.jpg" alt="ICPR 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.5334/tismir.157"><img src="http://stdm.github.io/images/papers/TISMIR_2023.jpg" alt="TISMIR 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/ACCESS.2022.3202639"><img src="http://stdm.github.io/images/papers/Access_2022.jpg" alt="Access 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://dx.doi.org/10.1109/ACCESS.2024.3404834"><img src="http://stdm.github.io/images/papers/Access_2024.jpg" alt="Access 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

An ongoing programme addresses the computational reading of printed musical scores and document images, i.e., document recognition. The [DeepScores](https://doi.org/10.21256/zhaw-4255) (ICPR'18a) and [DeepScoresV2](https://stdm.github.io/downloads/papers/ICPR_2020.pdf) (ICPR'20) datasets are among the largest for tiny, densely packed object detection, enabling systematic benchmarking on musical notation. The associated [Deep Watershed Detector](https://doi.org/10.21256/zhaw-3760) (ISMIR'18) demonstrated a novel instance segmentation approach for overlapping small objects. A [2024 TISMIR journal paper](https://doi.org/10.5334/tismir.157) reports real-world deployment, showing a substantial performance gap on digitised historical scores. Parallel work applied FCNNs to [newspaper article segmentation](https://doi.org/10.21256/zhaw-1533) and CNNs to [formula detection](https://doi.org/10.1109/ACCESS.2022.3202639) and [recognition](https://dx.doi.org/10.1109/ACCESS.2024.3404834). A new [preprint](https://arxiv.org/abs/2507.08458) draws on this background and introduces a new theory and first empirical results towards building document foundation models beyond optical character recognition (OCR) also for complex document typers like floor plans and engineering drawings.

| Paper | Key finding / message |
|---|---|
| [ICPR'18a](https://doi.org/10.21256/zhaw-4255) / [ICPR'20 *DeepScores(V2)*](https://stdm.github.io/downloads/papers/ICPR_2020.pdf) | Standard detectors fail on tiny, high-density objects; the dataset surfaces the gap and motivates specialised architectures. |
| [ISMIR'18 *Deep Watershed Detector*](https://doi.org/10.21256/zhaw-3760) | Energy-based instance segmentation via watershed post-processing achieves state-of-the-art on polyphonic music object detection. |
| [TISMIR'24 *Real World Music Object Recognition*](https://doi.org/10.5334/tismir.157) | Substantial performance gap versus synthetic data; domain adaptation is key for real OMR deployment. |
| [ArXiv'25 *Document Recognition as Tramscriptiion*](https://arxiv.org/abs/2507.08458) | Document recognition shouldn't be viewed as isolated computer vision tasks, but as end-to-end transcription of a full information; this view leads to rules for inductive bias design that allow the creation of document foundation models. |
</details>


<details markdown="1">
<summary><b>Medical image analysis</b></summary>
*~2021–ongoing: growing interdisciplinary programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://stdm.github.io/downloads/papers/CISP_BMEI_2021.pdf"><img src="http://stdm.github.io/images/papers/CISP_BMEI_2021.jpg" alt="CISP BMEI 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3390/jimaging8080222"><img src="http://stdm.github.io/images/papers/JImaging_2022.jpg" alt="JImaging 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/AAPM_2022.pdf"><img src="http://stdm.github.io/images/papers/AAPM_2022.jpg" alt="AAPM 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1002/mp.16405"><img src="http://stdm.github.io/images/papers/MedPhys_2023.jpg" alt="MedPhys 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/BioMed_2024.pdf"><img src="http://stdm.github.io/images/papers/BioMed_2024.jpg" alt="BioMed 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1038/s41598-024-64855-2"><img src="http://stdm.github.io/images/papers/SR_2024.jpg" alt="Sci Reports 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS66131.2025.00008"><img src="http://stdm.github.io/images/papers/SDS_2025b.jpg" alt="SDS 2025b" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ISBI_2026.pdf"><img src="http://stdm.github.io/images/papers/ISBI_2026.jpg" alt="ISBI 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A growing body of work addresses clinical imaging across four sub-themes: (a) *cross-domain generalisation* — [PrepNet](https://stdm.github.io/downloads/papers/CISP_BMEI_2021.pdf) homogenises heterogeneous CT scanners; [unsupervised domain adaptation](https://doi.org/10.3390/jimaging8080222) with a "domain sanity loss" detects vertebrae across scanner vendors; (b) *motion artefact correction* in CBCT ([MedPhys'23](https://doi.org/10.1002/mp.16405), top-viewed Wiley article); (c) *cell segmentation* for stain-free thyroid cancer diagnosis ([Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2)); (d) *inductive bias design* — Hounsfield unit priors enable data-efficient CT segmentation within a single clinic ([SDS'25b](https://doi.org/10.1109/SDS66131.2025.00008), Best Paper Award). The unifying theme is encoding domain knowledge as inductive biases to overcome data scarcity.

| Paper | Key finding / message |
|---|---|
| [Amirian et al., MedPhys'23](https://doi.org/10.1002/mp.16405) (Top-Viewed) | Deep CNNs reduce motion artefacts in 4D-CBCT to clinically acceptable levels, cutting processing from hours to seconds. |
| [Sager et al., JImaging'22](https://doi.org/10.3390/jimaging8080222) | A "domain sanity loss" achieves robust vertebra detection across different scanner vendors without paired training data. |
| [Jermain et al., Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2) | DL cell segmentation on rapid optical cytopathology images matches standard pathology accuracy for thyroid cancer. |
| [Meyer et al., SDS'25b](https://doi.org/10.1109/SDS66131.2025.00008) (Best Paper) | Hounsfield unit value ranges, a standard radiological prior, enable data-efficient CT segmentation trained within a single clinic. |
</details>


<details markdown="1">
<summary><b>AI Ethics & societal implications</b></summary>
*~2021–ongoing: normative and empirical strand*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" alt="AI Ethics 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s43681-023-00408-z"><img src="http://stdm.github.io/images/papers/AIEthics_2023.jpg" alt="AI Ethics 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s43681-026-01042-1"><img src="http://stdm.github.io/images/papers/AIEthics_2026.jpg" alt="AI Ethics 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" alt="PMM 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/GRW_2025.pdf"><img src="http://stdm.github.io/images/papers/GRW_2025.jpg" alt="GRW 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A distinct thread examines the ethical and societal dimensions of AI. The [2021 AI and Ethics paper](https://doi.org/10.1007/s43681-021-00108-6) on face recognition demonstrates empirically that *blinding a model to sensitive attributes does not reduce bias*, directly challenging a widely proposed de-biasing strategy. The [2023 AI and Ethics paper](https://link.springer.com/article/10.1007/s43681-023-00408-z) proposes a systematic work programme for the humanities to assess deep learning. The [2026 AI and Ethics paper](https://link.springer.com/article/10.1007/s43681-026-01042-1) establishes that the *stochastic nature of ML training has direct safety implications* for high-consequence deployments. The invited [PMM'26 paper](https://doi.org/10.1080/09540962.2025.2541304) proposes an evidence-based framework for AI risk assessment in public policy, arguing against worldview-induced AI fears.

| Paper | Key finding / message |
|---|---|
| [Wehrli et al., AI&Ethics'21](https://doi.org/10.1007/s43681-021-00108-6) | Model awareness of sensitive features and demographic accuracy disparity are empirically uncorrelated, hence blinding is not a valid de-biasing technique. |
| [Segessenmann et al., AI&Ethics'23](https://link.springer.com/article/10.1007/s43681-023-00408-z) | A structured humanities-informed programme for critically assessing DL systems across epistemology, ethics, and societal impact. |
| [Stadelmann et al., AI&Ethics'26](https://link.springer.com/article/10.1007/s43681-026-01042-1) | ML's inherent stochasticity must be explicitly accounted for in safety engineering; one way of doing so is with co-learning. |
</details>


<details markdown="1">
<summary><b>Theoretical foundations of intelligence</b></summary>
*~2022–ongoing: theoretical / foundational strand*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://arxiv.org/abs/2205.00002"><img src="http://stdm.github.io/images/papers/ArXiv_2022.jpg" alt="Theory Natural Intelligence" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/KogWis_2022.pdf"><img src="http://stdm.github.io/images/papers/KogWis_2022.jpg" alt="KogWis 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://icml.cc/virtual/2025/poster/44452"><img src="http://stdm.github.io/images/papers/ICML_2025.jpg" alt="ICML 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1162/NECO.a.1505"><img src="http://stdm.github.io/images/papers/NeuralComput_2025.jpg" alt="Neural Computation 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3389/fcomp.2025.1644044"><img src="http://stdm.github.io/images/papers/Frontiers_2025.jpg" alt="Frontiers 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

In collaboration with Christoph von der Malsburg (Frankfurt) and Benjamin Grewe (ETH Zurich), a theoretical programme investigates why natural intelligence is so data-efficient compared to current AI. The central argument in [*"A Theory of Natural Intelligence"*](https://arxiv.org/abs/2205.00002) (arXiv'22) is that both brain and natural environment are highly structured and that this mutual structural regularity acts as the key inductive bias enabling rapid, generalising learning via self-organised "net fragments." The [Neural Computation'26 paper](https://doi.org/10.1162/NECO.a.1505) instantiates the cooperative network architecture as a concrete instance of this theory of a a next level of AI could be build. At [ICML'25](https://icml.cc/virtual/2025/poster/44452), Saponati et al. showed that Transformer self-attention develops symmetry and directionality structures during training, informing deeper understanding of current ML methods. 

| Paper | Key finding / message |
|---|---|
| [von der Malsburg, Stadelmann, Grewe, arXiv'22](https://arxiv.org/abs/2205.00002) | Brain and environment are highly structured; self-organised "net fragments" serve as the structural inductive bias enabling data-efficient natural learning. |
| [Saponati, Sager et al., ICML'25](https://icml.cc/virtual/2025/poster/44452) | Transformers' self-attention develops symmetry and directionality structures during training, theoretically grounding attempts to increase training efficiency through initialization tricks. |
| [Sager et al., Neural Computation'26](https://doi.org/10.1162/NECO.a.1505) | The cooperative network architecture instantiates net-fragment theory; learns structured representations with strong few-shot generalisation. |
</details>


<details markdown="1">
<summary><b>Industrial AI applications</b></summary>
*~2019–ongoing: applied programme across multiple industrial domains*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://stdm.github.io/downloads/papers/AVHRC_2020.pdf"><img src="http://stdm.github.io/images/papers/AVHRC_2020.jpg" alt="AVHRC 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/SDS_2020.pdf"><img src="http://stdm.github.io/images/papers/SDS_2020.jpg" alt="SDS 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.geothermics.2024.103012"><img src="http://stdm.github.io/images/papers/Geothermics_2024.jpg" alt="Geothermics 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS60720.2024.00027"><img src="http://stdm.github.io/images/papers/SDS_2024c.jpg" alt="SDS 2024c" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/978-3-031-71602-7_27"><img src="http://stdm.github.io/images/papers/ANNPR_2024.jpg" alt="ANNPR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.isci.2025.113400"><img src="http://stdm.github.io/images/papers/iScience_2025.png" alt="iScience 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS66131.2025.00022"><img src="http://stdm.github.io/images/papers/SDS_2025a.jpg" alt="SDS 2025a" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s00501-025-01563-y"><img src="http://stdm.github.io/images/papers/BHM_2025.jpg" alt="BHM 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A broad programme applies ML, including RL and representation learning, to industrial control and monitoring. Key domains include rail traffic ([SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf): RL-based train rescheduling), building energy optimisation ([ANNPR'24](https://doi.org/10.1007/978-3-031-71602-7_27)), injection-moulding process monitoring ([SDS'24c](https://doi.org/10.1109/SDS60720.2024.00027)), industrial process control via world models ([SDS'25a](https://doi.org/10.1109/SDS66131.2025.00022)), and geothermal reservoir uncertainty quantification ([Geothermics'24](https://doi.org/10.1016/j.geothermics.2024.103012)). The [iScience'25 paper](https://doi.org/10.1016/j.isci.2025.113400) synthesises lessons on human-AI interaction in safety-critical infrastructures, introducing co-learning as a development paradigm.

| Paper | Key finding / message |
|---|---|
| [Roost et al., SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf) (Best Poster) | Multi-agent RL improves train rescheduling; sample efficiency and inter-agent communication are the key bottlenecks for real rail deployment. |
| [Yan et al., SDS'25a](https://doi.org/10.1109/SDS66131.2025.00022) | World-model-based RL enables industrial process control from limited real data by leveraging a learned environment model for planning. |
| [Mussi et al., iScience'25](https://doi.org/10.1016/j.isci.2025.113400) | Human-AI teaming in safety-critical systems requires trust calibration, explainability, and explicit workload allocation, resulting in co-learning architectures — purely autonomous AI is inappropriate in regulated contexts. |
</details>


<details markdown="1">
<summary><b>Graph neural networks for pattern recognition</b></summary>
*~2022–2026: methodical deep dive*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.1145/3555776.3578600"><img src="http://stdm.github.io/images/papers/GMLR_2023.jpg" alt="GMLR 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patrec.2024.09.009"><img src="http://stdm.github.io/images/papers/PRL_2024b.jpg" alt="PRL 2024b" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/S+SSPR_2024.pdf"><img src="http://stdm.github.io/images/papers/S+SSPR_2024.jpg" alt="S+SSPR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patcog.2025.112786"><img src="http://stdm.github.io/images/papers/PR_2025.png" alt="Pattern Recognition 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/NNICE_2026.pdf"><img src="http://stdm.github.io/images/papers/NNICE_2026.jpg" alt="NNICE 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A self-contained thread, developed in collaboration with Marcello Pelillo (Venice), investigates graph-based deep learning, particularly the design of expressive yet computationally efficient *graph pooling* operators for graph classification. Key contributions include [Quasi-CliquePool](https://doi.org/10.1145/3555776.3578600) (SAC'23), [Hierarchical Glocal Attention Pooling](https://doi.org/10.1016/j.patrec.2024.09.009) (PRL'24), [Multi-View Pooling via Dominant Sets](https://doi.org/10.1016/j.patcog.2025.112786) (Pattern Recognition'26), and [Community-Hop](https://stdm.github.io/downloads/papers/S+SSPR_2024.pdf) for node classification (S+SSPR'24). These methods consistently outperform prior pooling approaches while maintaining interpretability through their graph-theoretic foundations.

| Paper | Key finding / message |
|---|---|
| [Ali et al., PRL'24 *Hierarchical Glocal Attention Pooling*](https://doi.org/10.1016/j.patrec.2024.09.009) | Combining global graph structure with local neighbourhood attention in hierarchical pooling achieves state-of-the-art graph classification. |
| [Ali et al., Pattern Recognition'26 *Multi-View via Dominant Sets*](https://doi.org/10.1016/j.patcog.2025.112786) | Treating pooling as a dominant-set clustering problem provides a principled, parameter-efficient alternative to learned pooling operators. |
</details>



<a name="practice"></a>
## Examples of translation into practice

The table below maps concrete, practitioner-relevant examples from across the research portfolio to their domain, method, and key practical takeaway.

| | Application | Domain | What was done | Practical takeaway |
|---|---|---|---|---|
| <a href="https://doi.org/10.1007/978-3-319-99978-4"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" style="height:60px; width:auto;"/></a> | **Face-ID verification product** | Identity & security | Full production pipeline: orientation detection, image quality assessment, anti-spoofing (3-method ensemble), face matching, user guidance. ([ANNPR'18d](https://doi.org/10.1007/978-3-319-99978-4)) | A single ML model is never enough in production; wrapping in auxiliary quality and security modules is mandatory. |
| <a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" style="height:60px; width:auto;"/></a> | **Newspaper article segmentation** | Media / publishing | FCNNs segment printed newspaper pages into articles at >10 000 pages/day for a media monitoring company. ([ICDAR'17](https://doi.org/10.21256/zhaw-1533)) | Excluding non-article regions and handling layout diversity are the dominant engineering challenges, not the core model. |
| <a href="https://doi.org/10.1002/mp.16405"><img src="http://stdm.github.io/images/papers/MedPhys_2023.jpg" style="height:60px; width:auto;"/></a> | **Radiotherapy CBCT correction** | Medical physics | Deep CNNs reduce motion artefacts in cone-beam CT scans, improving image quality for treatment planning. ([MedPhys'23](https://doi.org/10.1002/mp.16405), *Top-Viewed*) | DL replaces iterative reconstruction, cutting processing from hours to seconds at equivalent image quality. |
| <a href="https://doi.org/10.1038/s41598-024-64855-2"><img src="http://stdm.github.io/images/papers/SR_2024.jpg" style="height:60px; width:auto;"/></a> | **Thyroid cancer cytology** | Pathology / oncology | Cell segmentation on rapid optical cytopathology images (no staining required) enables real-time intraoperative diagnosis. ([Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2)) | Stain-free optical biopsy becomes clinically feasible; DL cell segmentation matches standard pathology accuracy. |
| <a href="https://stdm.github.io/downloads/papers/SDS_2020.pdf"><img src="http://stdm.github.io/images/papers/SDS_2020.jpg" style="height:60px; width:auto;"/></a> | **Train rescheduling** | Rail / logistics | Multi-agent RL agents reschedule delayed trains, collaborating via communication to restore timetable adherence. ([SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf), *Best Poster*) | RL outperforms rule-based schedulers; sample efficiency and communication are the bottlenecks for real deployment. |
| <a href="https://doi.org/10.1007/978-3-031-71602-7_27"><img src="http://stdm.github.io/images/papers/ANNPR_2024.jpg" style="height:60px; width:auto;"/></a> | **Building energy optimisation** | Energy / smart buildings | RL agent controls HVAC to minimise energy consumption while satisfying occupant comfort constraints, trained in simulation. ([ANNPR'24](https://doi.org/10.1007/978-3-031-71602-7_27)) | Simulation-to-real transfer is feasible with proper domain randomisation; RL substantially outperforms rule-based controllers. |
| <a href="https://doi.org/10.1016/j.geothermics.2024.103012"><img src="http://stdm.github.io/images/papers/Geothermics_2024.jpg" style="height:60px; width:auto;"/></a> | **Geothermal reservoir modelling** | Energy / geology | Ensemble deep learning quantifies uncertainty in geothermal reservoir properties from sparse borehole data. ([Geothermics'24](https://doi.org/10.1016/j.geothermics.2024.103012)) | Probabilistic DL models provide actionable uncertainty bounds for drilling decisions with very limited training data. |
| <a href="https://doi.org/10.1063/5.0139707"><img src="http://stdm.github.io/images/papers/APLML_2023.jpg" style="height:60px; width:auto;"/></a> | **Solar cell characterisation** | Materials / clean energy | Deep ensemble inverse models estimate physical material parameters of organic solar cells from electroluminescence images. ([APLML'23](https://doi.org/10.1063/5.0139707); [SDS'21b](https://stdm.github.io/downloads/papers/SDS_2021b.pdf), *Best Paper*) | Ensembles trained on synthetic simulation data reliably invert physical imaging models; uncertainty quantification is essential. |
| <a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" style="height:60px; width:auto;"/></a> | **Bias testing in face recognition** | Ethics / HR / law enforcement | Empirically tested whether "blinding" a face recognition model to gender/race reduces accuracy disparity across demographic groups. ([AI&Ethics'21](https://doi.org/10.1007/s43681-021-00108-6)) | Blinding does *not* reduce bias. Organisations cannot rely on simple attribute removal as a fairness guarantee. |
| <a href="https://dx.doi.org/10.1109/ACCESS.2024.3404834"><img src="http://stdm.github.io/images/papers/Access_2024.jpg" style="height:60px; width:auto;"/></a> | **Mathematical formula recognition** | Publishing / accessibility | Data-centric approach with the FormulaNet benchmark achieves reliable printed formula detection and recognition. ([Access'22](https://doi.org/10.1109/ACCESS.2022.3202639); [Access'24](https://dx.doi.org/10.1109/ACCESS.2024.3404834)) | Data quality and annotation consistency matter more than model architecture; the bottleneck is the training set, not the network. |
| <a href="https://doi.org/10.1109/ACCESS.2023.3349132"><img src="http://stdm.github.io/images/papers/Access_2023.jpg" style="height:60px; width:auto;"/></a> | **Industrial anomaly detection** | Manufacturing / IoT | Comprehensive survey of deep transfer learning for anomaly detection in industrial time series, covering 150+ papers. ([Access'23/24](https://doi.org/10.1109/ACCESS.2023.3349132), *>100 citations*) | Pre-trained models fine-tuned with as few as 10–50 labelled examples; transfer learning is the practical standard for industrial sensor data. |
| <a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" style="height:60px; width:auto;"/></a> | **AI risk assessment for public policy** | Governance / regulation | Evidence-based framework mapping technical ML properties (stochasticity, distributional shift) to policy-relevant risk categories. ([PMM'26](https://doi.org/10.1080/09540962.2025.2541304); [AI&Ethics'26](https://link.springer.com/article/10.1007/s43681-026-01042-1)) | Regulators need technically grounded criteria; the stochastic nature of ML training must be acknowledged in safety cases. |



<a name="contributions"></a>
## Main scientific contributions

<details markdown="1">
<summary><b>Three strong claims for scientific breakthrough</b></summary>

<br>

The following three contributions represent the group's most coherent and fundable scientific claims — each with a clear arc, a body of evidence, and an open trajectory.

---

### 1. Neural Speaker Recognition and Diarization
*2004 – 2018, with ongoing relevance as a methodological platform*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://stdm.github.io/downloads/papers/ICASSP_2006.pdf"><img src="http://stdm.github.io/images/papers/ICASSP_2006.jpg" alt="ICASSP 2006" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465"><img src="http://stdm.github.io/images/papers/PhdThesis_2010.jpg" alt="PhD Thesis 2010" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3761"><img src="http://stdm.github.io/images/papers/MLSP_2016.jpg" alt="MLSP 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3762"><img src="http://stdm.github.io/images/papers/MLSP_2017.jpg" alt="MLSP 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

Starting from first principles in signal processing and statistical modelling, this line of work built a comprehensive account of how to identify and cluster speakers automatically from audio — the task known as speaker diarization. The early contributions ([ICASSP'06](https://stdm.github.io/downloads/papers/ICASSP_2006.pdf)) introduced fast and robust speaker clustering using Earth Mover's Distance and MixMax models, operating on real-world degraded recordings without prior knowledge of the number of speakers. The [doctoral dissertation (2010)](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) provided the most complete treatment of voice modelling methods for speaker recognition of its time, systematically comparing generative and discriminative approaches across diverse corpora.

The line was transformed by deep learning: [MLSP'16](https://doi.org/10.21256/zhaw-3761) demonstrated that convolutional networks trained on spectrograms could learn speaker-discriminative embeddings that cluster across unseen recordings without retraining — one of the early demonstrations of this paradigm before x-vectors became standard practice. The follow-up [MLSP'17](https://doi.org/10.21256/zhaw-3762) refined the approach through metric learning objectives directly optimised for clustering quality. Together, this body of work documents a full methodological cycle from classical statistical approaches to neural representations, establishing the group as a European reference point in audio-based biometric intelligence.

---

### 2. Dense Small-Object Detection: DeepScores and the Deep Watershed Detector
*2017 – 2025, with DeepScores as an ongoing community resource*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" alt="ICDAR 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-4255"><img src="http://stdm.github.io/images/papers/ICPR_2018a.jpg" alt="ICPR 2018 – DeepScores" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3760"><img src="http://stdm.github.io/images/papers/ISMIR_2018.jpg" alt="ISMIR 2018 – DWD" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.5334/tismir.157"><img src="http://stdm.github.io/images/papers/TISMIR_2023.jpg" alt="TISMIR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patcog.2025.112786"><img src="http://stdm.github.io/images/papers/PR_2025.png" alt="Pattern Recognition 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

This is the group's strongest claim to a core computer vision contribution. Standard object detectors — YOLO, SSD, Faster R-CNN — share a structural failure mode when applied to images containing large numbers of very small, densely packed objects: grid-based anchor mechanisms impose spatial constraints that prevent detecting multiple co-located objects regardless of training data or hyperparameter tuning. [DeepScores (ICPR'18)](https://doi.org/10.21256/zhaw-4255), with 80 million labelled objects across 300,000 high-resolution images of music notation, makes this failure mode precisely measurable. At several orders of magnitude larger in object count than PASCAL VOC or MS-COCO, it poses the dense small-object detection problem to the broader computer vision community rather than to optical music recognition alone.

The [Deep Watershed Detector (ISMIR'18)](https://doi.org/10.21256/zhaw-3760) addresses this structurally: instead of bounding-box regression from a spatial grid, it predicts a dense energy map where object centres appear as local peaks extracted by the watershed transform. This makes it conceptually an anchor-free dense detector — contemporaneous with CornerNet (ECCV'18) but derived from different mathematical foundations that provide a clean topological justification for handling crowded scenes. A model trained on synthetically rendered scores generalised directly to handwritten notation (MUSCIMA++) without retraining, a strong out-of-distribution result. Subsequent work ([TISMIR'24](https://doi.org/10.5334/tismir.157), [PR'25](https://doi.org/10.1016/j.patcog.2025.112786)) extended and validated the approach on real-world scores, with methodology that transfers to satellite imagery, document analysis, and histopathology.

---

### 3. From Algorithmic Research to Societal Questions
*2018 – present, increasingly the group's primary intellectual orientation*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em;">
<a href="https://doi.org/10.1007/978-3-319-99978-4"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" alt="Deep Learning in the Wild" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://dx.doi.org/10.5445/IR/1000143637"><img src="http://stdm.github.io/images/papers/AoDSA_2022a.jpg" alt="Data Centrism 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" alt="AI Ethics 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-023-00408-z"><img src="http://stdm.github.io/images/papers/AIEthics_2023.jpg" alt="AI Ethics 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" alt="PMM 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-026-01042-1"><img src="http://stdm.github.io/images/papers/AIEthics_2026.jpg" alt="AI Ethics 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

The third contribution is not a method but a movement: the group has systematically traced what happens when machine learning results exit the research lab and encounter real human contexts, producing original scientific arguments at each stage of that transition. The invited position paper [Deep Learning in the Wild (ANNPR'18)](https://doi.org/10.1007/978-3-319-99978-4) opened this line by cataloguing the gap between benchmark conditions and deployment realities, providing a taxonomy of failure modes that predates much of the later "reproducibility crisis" literature in ML. The [Data Centrism paper (AoDSA'22)](https://dx.doi.org/10.5445/IR/1000143637) went further, arguing that data — not algorithms or models — is the primary scientific object of data science, with direct implications for how the discipline should evaluate its own contributions.

On the applied side, the [AI & Ethics (2021)](https://doi.org/10.1007/s43681-021-00108-6) bias study showed quantitatively that demographic awareness in face recognition design does not translate to reduced bias at deployment. [Assessing Deep Learning (AI&Ethics'23)](https://doi.org/10.1007/s43681-023-00408-z) proposed a humanities-grounded framework for evaluating AI systems beyond technical metrics. Most recently, [PMM'26](https://doi.org/10.1080/09540962.2025.2541304) and [AI&Ethics'26](https://doi.org/10.1007/s43681-026-01042-1) formalised how intrinsic ML properties — stochasticity of training, distributional shift — map to policy-relevant risk categories, giving regulators technically grounded criteria that go beyond checklist compliance.

</details>
