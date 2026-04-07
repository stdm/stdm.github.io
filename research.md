---
title: Research
layout: page
comments: false
---

The [Machine Perception and Cognition group](https://stdm.github.io/home/#group) occupies a distinctive position at the intersection of applied and foundational AI research. It is firmly motivated by practical problems (ca. 80% of our research is joint work with practice partners), yet consistently engages fundamental questions about, e.g., what data science <em>is</em>, how natural intelligence works, and what ML's stochastic nature means for safety, publishing  at top venues regularly (ICML, Nature Scientific Reports, Pattern Recognition, AI and Ethics etc.). Below is a summary of some defining traits that emerge consistently across the [full publication record](https://stdm.github.io/homme/#publications) of >100 papers from >20 years (as of April 2026), serving as a key to our work. It is geared towards fellow researchers & engineers.

### TOC
1. [The mindset behind our work](#mindset)
2. [Research lines](#research)
3. [Examples of translation into practice](#practice)
4. [Main scientific contributions](#contributions)
5. [Ideas we'd love to work on in the future](#ideas)


<img alt="Thilo Stadelmann and Yann LeCun discussing world models and cowbell blues at the Swiss AI Award 2023 ceremony in Davos, Switzerland" src="http://stdm.github.io/images/stdm-lecun.jpg"/>


<a name="mindset"></a>
## The mindset behind our work

<div style="background:#f0f5fb; border:1px solid #bdd0e8; border-radius:6px; padding:20px 26px 14px; margin:1.2em 0 2em;">


<div style="display:grid; grid-template-columns:repeat(auto-fill, minmax(300px, 1fr)); gap:14px; margin-top:1em;">

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Principled pragmatism.</strong> Problems must matter outside the lab, but engineering alone is not enough. There is a recurring impulse to step back and ask "what general principle explains this?", leading to <a href="https://www.mdpi.com/2673-2688/1/4/31">design-pattern taxonomies</a>, a proposal for <a href="https://dx.doi.org/10.5445/IR/1000143637">data science's foundation</a>, a <a href="https://arxiv.org/abs/2205.00002">theory of natural intelligence</a>, or the <a href="https://doi.org/10.3390/educsci11070318">ATLAS teaching concept</a>.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Translator instinct.</strong> A substantial share of the output (e.g., the <a href="https://stdm.github.io/data-science-book/">Applied Data Science book</a> (with &gt;123 k readers), <a href="https://doi.org/10.1007/978-3-319-99978-4">"Deep Learning in the Wild"</a>, or <a href="https://doi.org/10.1080/09540962.2025.2541304">white papers for policymakers</a> explicitly closes the gap between what researchers know and what practitioners and regulators can act on.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Empirical honesty.</strong> Several of the strongest papers report negative or counter-intuitive findings: <a href="https://doi.org/10.1016/j.patrec.2024.03.016">DNNs for speaker recognition don't learn temporal voice features</a>; <a href="https://doi.org/10.1007/s43681-021-00108-6">blinding face-recognition models to sensitive attributes doesn't reduce demographic bias</a>; <a href="https://doi.org/10.3389/fcomp.2022.1041703">ImageNet-optimal architectures don't transfer across domains</a>.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Disciplinary self-consciousness.</strong> Unusual for a technical ML group, we invest sustained effort in defining what our own discipline fundamentally <em>is</em>. The <a href="https://dx.doi.org/10.5445/IR/1000143637">data-centrism paper</a>, the <a href="https://stdm.github.io/downloads/papers/ECSS_2013.pdf">ECSS</a> and <a href="https://doi.org/10.21256/zhaw-3759">HMD series</a>, or the <a href= "https://publikationen.bibliothek.kit.edu/1000146422">"Foundations of Data Science" overview</a> are acts of disciplinary self-definition.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Long arcs alongside rapid response.</strong> Some threads run for more than a decade (<a href="#speakerrec">speaker recognition</a>, <a href="#dromr">optical music recognition</a>, <a href="#datascience">applied data science</a>). Others respond quickly to emerging topics (<a href="https://doi.org/10.1109/SDS60720.2024.00036">LLM efficiency</a>, <a href="https://doi.org/10.1613/jair.1.19490">AI agents survey</a>, <a href="https://link.springer.com/article/10.1007/s43681-026-01042-1">stochasticity and safety</a>). A stable intellectual core with enough flexibility to engage new problems without losing continuity.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Genuinely interdisciplinary collaborators.</strong> Co-authors span, amongst others, <a href="https://doi.org/10.1002/mp.16405">radiologists</a>, <a href="https://doi.org/10.1063/5.0139707">physicists</a>, <a href="https://doi.org/10.1016/j.geothermics.2024.103012">geothermal engineers</a>, <a href="https://arxiv.org/abs/2205.00002">cognitive neuroscientists</a>, <a href="https://doi.org/10.5334/tismir.157">musicians</a>, <a href="https://doi.org/10.1007/s43681-021-00108-6">social workers</a>, <a href="https://stdm.github.io/downloads/papers/SDS_2020.pdf">transport engineers</a>, and <a href="https://link.springer.com/article/10.1007/s43681-023-00408-z">theologians</a>. Domain knowledge visibly shapes methodology in each case.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Applied science identity, worn lightly.</strong> The Fachhochschule mandate (problems must be real) is treated as the motivational inspiration, not a ceiling on ambition. <a href="https://icml.cc/virtual/2025/poster/44452">ICML papers</a> and <a href="https://doi.org/10.1162/NECO.a.1505">Neural Computation articles</a> coexist with <a href="https://stdm.github.io/downloads/papers/SDS_2023a.pdf">industrial reports</a> and <a href="https://stdm.github.io/data-science-book/">practitioner handbooks</a>.
</div>

<div style="background:white; border-left:4px solid #2c5f8a; border-radius:3px; padding:10px 14px; box-shadow:0 1px 3px rgba(0,0,0,0.07);">
<strong>Education as a research topic.</strong> Teaching AI is treated as an object of scholarly inquiry, not just a duty. The <a href="https://doi.org/10.3390/educsci11070318">ATLAS concept on hybrid AI education</a>, and the <a href="https://stdm.github.io/downloads/papers/Buergenstock_2023.pdf">Bürgenstock higher education workshop</a> reflect a conviction that how we teach and how we build organizations of higher education shapes what the field becomes.
</div>

</div><!-- trait grid -->
</div><!-- character box -->


<a name="research"></a>
## Research lines

Being motivated by real-world pattern recognition problems (how perceptions are formed from sensory input and cognitively translated into reasonable actions) leads to a suprinsingly broad field of use cases and industries amidst a stable core of methodological focal points. Here's an overview of sub-disciplines our inquiry contributes to.


<details markdown="1">
<summary><b>Industrial AI applications</b></summary>
*~2019-ongoing: applied programme across multiple industrial domains*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://stdm.github.io/downloads/papers/AVHRC_2020.pdf"><img src="http://stdm.github.io/images/papers/AVHRC_2020.jpg" alt="AVHRC 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/SDS_2020.pdf"><img src="http://stdm.github.io/images/papers/SDS_2020.jpg" alt="SDS 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.geothermics.2024.103012"><img src="http://stdm.github.io/images/papers/Geothermics_2024.jpg" alt="Geothermics 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS60720.2024.00027"><img src="http://stdm.github.io/images/papers/SDS_2024c.jpg" alt="SDS 2024c" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/978-3-031-71602-7_27"><img src="http://stdm.github.io/images/papers/ANNPR_2024.jpg" alt="ANNPR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.isci.2025.113400"><img src="http://stdm.github.io/images/papers/iScience_2025.png" alt="iScience 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS66131.2025.00022"><img src="http://stdm.github.io/images/papers/SDS_2025a.jpg" alt="SDS 2025a" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s00501-025-01563-y"><img src="http://stdm.github.io/images/papers/BHM_2025.jpg" alt="BHM 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A broad programme applies ML, including RL and representation learning, to industrial problems like control and monitoring. Domains include visual quality control ([ANNPR'18 invited paper](https://link.springer.com/book/10.1007/978-3-319-99978-4)), predictive maintenance ([Beyond ImageNet chapter](https://doi.org/10.1007/978-3-030-11821-1_12)), rail traffic ([SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf): RL-based train rescheduling), building energy optimisation ([ANNPR'24](https://doi.org/10.1007/978-3-031-71602-7_27)), injection-moulding process monitoring ([SDS'24c](https://doi.org/10.1109/SDS60720.2024.00027)), industrial process control via world models ([SDS'25a](https://doi.org/10.1109/SDS66131.2025.00022)), and geothermal reservoir uncertainty quantification ([Geothermics'24](https://doi.org/10.1016/j.geothermics.2024.103012)). The [iScience'25 paper](https://doi.org/10.1016/j.isci.2025.113400) synthesises lessons on human-AI interaction in safety-critical infrastructures, introducing co-learning as a development paradigm.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Roost et al., SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf) (Best Poster) | Multi-agent RL improves train rescheduling; sample efficiency and inter-agent communication are the key bottlenecks for real rail deployment. |
| [Yan et al., SDS'25a](https://doi.org/10.1109/SDS66131.2025.00022) | World-model-based RL enables industrial process control from limited real data by leveraging a learned environment model for planning. |
| [Mussi et al., iScience'25](https://doi.org/10.1016/j.isci.2025.113400) | Human-AI teaming in safety-critical systems requires trust calibration, explainability, and explicit workload allocation, resulting in co-learning architectures. |

</div>
</details>


<details markdown="1">
<a name="dromr"></a>
<summary><b>Document recognition & optical music recognition</b></summary>
*~2017-ongoing: dedicated dataset and methods programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" alt="ICDAR 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-4255"><img src="http://stdm.github.io/images/papers/ICPR_2018a.jpg" alt="ICPR 2018a" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3760"><img src="http://stdm.github.io/images/papers/ISMIR_2018.jpg" alt="ISMIR 2018" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/WoRMS_2018.pdf"><img src="http://stdm.github.io/images/papers/WoRMS_2018.jpg" alt="WoRMS 2018" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ICPR_2020.pdf"><img src="http://stdm.github.io/images/papers/ICPR_2020.jpg" alt="ICPR 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.5334/tismir.157"><img src="http://stdm.github.io/images/papers/TISMIR_2023.jpg" alt="TISMIR 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/ACCESS.2022.3202639"><img src="http://stdm.github.io/images/papers/Access_2022.jpg" alt="Access 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://dx.doi.org/10.1109/ACCESS.2024.3404834"><img src="http://stdm.github.io/images/papers/Access_2024.jpg" alt="Access 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

An ongoing programme addresses document recognition, i.e., the computational reading of document images like printed musical scores. The [DeepScores](https://doi.org/10.21256/zhaw-4255) (ICPR'18a) and [DeepScoresV2](https://stdm.github.io/downloads/papers/ICPR_2020.pdf) (ICPR'20) datasets are among the largest for tiny, densely packed object detection, enabling systematic benchmarking on musical notation. The associated [Deep Watershed Detector](https://doi.org/10.21256/zhaw-3760) (ISMIR'18) demonstrated a novel instance segmentation approach for overlapping small objects. A [2024 TISMIR journal paper](https://doi.org/10.5334/tismir.157) reports real-world deployment, showing a substantial performance gap on digitised historical scores. Parallel work applied FCNNs to [newspaper article segmentation](https://doi.org/10.21256/zhaw-1533) and CNNs to [formula detection](https://doi.org/10.1109/ACCESS.2022.3202639) and [recognition](https://dx.doi.org/10.1109/ACCESS.2024.3404834). A new [preprint](https://arxiv.org/abs/2507.08458) draws on this background and introduces a new theory and first empirical results towards building document foundation models beyond optical character recognition (OCR) also for complex document typers like floor plans and engineering drawings.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [ICPR'18a](https://doi.org/10.21256/zhaw-4255) / [ICPR'20 *DeepScores(V2)*](https://stdm.github.io/downloads/papers/ICPR_2020.pdf) | Standard detectors fail on tiny, high-density objects; the datasets surfaces the gap and motivate specialised architectures. |
| [ISMIR'18 *Deep Watershed Detector*](https://doi.org/10.21256/zhaw-3760) | Energy-based instance segmentation via watershed post-processing achieves state-of-the-art on polyphonic music object detection. |
| [TISMIR'24 *Real World Music Object Recognition*](https://doi.org/10.5334/tismir.157) | Domain adaptation and confidence estimation is key for real OMR deployment. |
| [ArXiv'25 *Document Recognition as Tramscriptiion*](https://arxiv.org/abs/2507.08458) | Document recognition shouldn't be viewed as isolated computer vision tasks, but as end-to-end transcription of full information; this view leads to rules for inductive bias design that allow the creation of document foundation models. |

</div>
</details>


<details markdown="1">
<summary><b>Applied deep learning: from benchmarks to production</b></summary>
*~2016-ongoing: centrepiece applied-ML research programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.1007/978-3-319-99978-4"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" alt="DL in the Wild" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/SDS_2019.pdf"><img src="http://stdm.github.io/images/papers/SDS_2019.jpg" alt="SDS 2019" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://www.mdpi.com/2673-2688/1/4/31"><img src="http://stdm.github.io/images/papers/AI_2020.jpg" alt="AI 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/TAILOR_2020.pdf"><img src="http://stdm.github.io/images/papers/TAILOR_2020.jpg" alt="TAILOR 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3389/fcomp.2022.1041703"><img src="http://stdm.github.io/images/papers/Frontiers_2022.jpg" alt="Frontiers 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A distinctive contribution is the systematic study of the gap between benchmark-driven research and real-world deployment. The invited paper [*"Deep Learning in the Wild"*](https://doi.org/10.1007/978-3-319-99978-4) (ANNPR'18) distils lessons from six production use cases. The companion book chapter [*"Beyond ImageNet"*](https://stdm.github.io/downloads/papers/ADS_2019_DeepLearning.pdf) (Springer, 2019) generalises these into transferable principles. The MDPI AI paper on ["Design Patterns for Resource-Constrained Automated Deep-Learning Methods"](https://www.mdpi.com/2673-2688/1/4/31) (2020) synthesises the methodological takeaways into reusable patterns. The [Frontiers'22 paper](https://doi.org/10.3389/fcomp.2022.1041703) closes the loop empirically, showing that ImageNet-optimal architectures fail to transfer across domains.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Stadelmann et al., ANNPR'18d](https://doi.org/10.1007/978-3-319-99978-4) | Real deployment requires wrapping core DL models in ensembles of auxiliary modules; benchmark accuracy is necessary but not sufficient. |
| [Stadelmann et al., ADS ch. *Beyond ImageNet* (2019)](https://stdm.github.io/downloads/papers/ADS_2019_DeepLearning.pdf) | Most industrial DL projects require domain-specific data curation, loss shaping, and calibration absent from canonical ImageNet training. |
| [Tuggener et al., MDPI AI 2020 *Design Patterns*](https://www.mdpi.com/2673-2688/1/4/31) | Seven reusable design patterns cover the majority of resource-constrained AutoML scenarios and lead to top-5 results in international AutoML competitions. |
| [Tuggener et al., Frontiers 2022](https://doi.org/10.3389/fcomp.2022.1041703) | CNN architectures optimised on ImageNet do not reliably transfer across domains, hence architecture search must be domain-aware. |

</div>
</details>


<details markdown="1">
<summary><b>Medical image analysis</b></summary>
*~2021-ongoing: growing interdisciplinary programme*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://stdm.github.io/downloads/papers/CISP_BMEI_2021.pdf"><img src="http://stdm.github.io/images/papers/CISP_BMEI_2021.jpg" alt="CISP BMEI 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3390/jimaging8080222"><img src="http://stdm.github.io/images/papers/JImaging_2022.jpg" alt="JImaging 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/AAPM_2022.pdf"><img src="http://stdm.github.io/images/papers/AAPM_2022.jpg" alt="AAPM 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1002/mp.16405"><img src="http://stdm.github.io/images/papers/MedPhys_2023.jpg" alt="MedPhys 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/BioMed_2024.pdf"><img src="http://stdm.github.io/images/papers/BioMed_2024.jpg" alt="BioMed 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1038/s41598-024-64855-2"><img src="http://stdm.github.io/images/papers/SR_2024.jpg" alt="Sci Reports 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1109/SDS66131.2025.00008"><img src="http://stdm.github.io/images/papers/SDS_2025b.jpg" alt="SDS 2025b" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ISBI_2026.pdf"><img src="http://stdm.github.io/images/papers/ISBI_2026.jpg" alt="ISBI 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A growing body of work addresses clinical imaging, e.g.: (a) *cross-domain generalisation*: [PrepNet](https://stdm.github.io/downloads/papers/CISP_BMEI_2021.pdf) homogenises heterogeneous CT scanners; (b) *motion artefact correction* in CBCT ([MedPhys'23](https://doi.org/10.1002/mp.16405), top-viewed Wiley article); (c) *cell segmentation* for stain-free thyroid cancer diagnosis ([Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2)); (d) *inductive bias design*: [unsupervised domain adaptation](https://doi.org/10.3390/jimaging8080222) with a "domain sanity loss" detects vertebrae across scanner vendors; Hounsfield unit priors enable data-efficient CT segmentation within a single clinic ([SDS'25b](https://doi.org/10.1109/SDS66131.2025.00008), Best Paper Award). The unifying theme is encoding domain knowledge as inductive biases to overcome data scarcity.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Amirian et al., MedPhys'23](https://doi.org/10.1002/mp.16405) (Top-Viewed) | Deep CNNs reduce motion artefacts in 4D-CBCT to clinically acceptable levels, cutting processing from hours to seconds. |
| [Sager et al., JImaging'22](https://doi.org/10.3390/jimaging8080222) | A "domain sanity loss" achieves robust vertebra detection across different scanner vendors without paired training data, bringing the need for in-house samples downm to ca. 10. |
| [Jermain et al., Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2) | DL cell segmentation on rapid optical cytopathology images matches standard pathology accuracy for thyroid cancer, enabling new workflows that might change the practice of cancer diagnosis worldwide. |
| [Meyer et al., SDS'25b](https://doi.org/10.1109/SDS66131.2025.00008) (Best Paper) | Hounsfield unit value ranges, a standard radiological prior, enable data-efficient CT segmentation trained within a single clinic: better accuracy with less than half the number of samples. |

</div>
</details>


<details markdown="1">
<summary><b>AI Ethics & societal implications</b></summary>
*~2021-ongoing: normative and empirical strand*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" alt="AI Ethics 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s43681-023-00408-z"><img src="http://stdm.github.io/images/papers/AIEthics_2023.jpg" alt="AI Ethics 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://link.springer.com/article/10.1007/s43681-026-01042-1"><img src="http://stdm.github.io/images/papers/AIEthics_2026.jpg" alt="AI Ethics 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" alt="PMM 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/GRW_2025.pdf"><img src="http://stdm.github.io/images/papers/GRW_2025.jpg" alt="GRW 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A distinct thread examines the ethical and societal dimensions of AI. The [2021 AI and Ethics paper](https://doi.org/10.1007/s43681-021-00108-6) on face recognition demonstrates empirically that *blinding a model to sensitive attributes does not reduce bias*, directly challenging a widely proposed de-biasing strategy. The [2023 AI and Ethics paper](https://link.springer.com/article/10.1007/s43681-023-00408-z) proposes a systematic work programme for the humanities to assess deep learning in its relationship to the human. The [2026 AI and Ethics paper](https://link.springer.com/article/10.1007/s43681-026-01042-1) establishes that the *stochastic nature of ML training has direct safety implications* for high-consequence deployments, and proposes co-learning for meaningful human control. The invited [PMM'26 paper](https://doi.org/10.1080/09540962.2025.2541304) proposes an evidence-based framework for AI risk assessment in public policy, arguing against worldview-induced AI fears.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Wehrli et al., AI&Ethics'21](https://doi.org/10.1007/s43681-021-00108-6) | Model awareness of sensitive features and demographic accuracy disparity are empirically uncorrelated, hence blinding is not a valid de-biasing technique. |
| [Segessenmann et al., AI&Ethics'23](https://link.springer.com/article/10.1007/s43681-023-00408-z) | A structured humanities-informed programme for critically assessing DL systems across epistemology, ethics, and societal impact. |
| [Stadelmann et al., AI&Ethics'26](https://link.springer.com/article/10.1007/s43681-026-01042-1) | ML's inherent stochasticity must be explicitly accounted for in safety engineering; one way of doing so is with co-learning. |

</div>
</details>


<details markdown="1">
<summary><b>Theoretical foundations of intelligence</b></summary>
*~2022-ongoing: theoretical / foundational strand*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://arxiv.org/abs/2205.00002"><img src="http://stdm.github.io/images/papers/ArXiv_2022.jpg" alt="Theory Natural Intelligence" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/KogWis_2022.pdf"><img src="http://stdm.github.io/images/papers/KogWis_2022.jpg" alt="KogWis 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://icml.cc/virtual/2025/poster/44452"><img src="http://stdm.github.io/images/papers/ICML_2025.jpg" alt="ICML 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1162/NECO.a.1505"><img src="http://stdm.github.io/images/papers/NeuralComput_2025.jpg" alt="Neural Computation 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3389/fcomp.2025.1644044"><img src="http://stdm.github.io/images/papers/Frontiers_2025.jpg" alt="Frontiers 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

In collaboration with Christoph von der Malsburg (Frankfurt) and Benjamin Grewe (ETH Zurich), a theoretical programme investigates why natural intelligence is so data-efficient compared to current AI. The central argument in [*"A Theory of Natural Intelligence"*](https://arxiv.org/abs/2205.00002) (arXiv'22) is that both brain and natural environment are highly structured and that this mutual structural regularity acts as the key inductive bias enabling rapid, generalising learning via self-organised "net fragments." The [Neural Computation'26 paper](https://doi.org/10.1162/NECO.a.1505) instantiates the cooperative network architecture as a concrete instance of this theory, hinting at how a next level of AI could be build. At the same time, our [ICML'25](https://icml.cc/virtual/2025/poster/44452) paper showed that Transformer self-attention develops symmetry and directionality structures during training, informing deeper understanding of current mainstream ML methods. 

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [von der Malsburg, Stadelmann, Grewe, arXiv'22](https://arxiv.org/abs/2205.00002) | Brain and environment are highly structured; self-organised "net fragments" serve as the structural inductive bias enabling data-efficient natural learning. |
| [Saponati, Sager et al., ICML'25](https://icml.cc/virtual/2025/poster/44452) | Transformers' self-attention develops symmetry and directionality structures during training, theoretically grounding attempts to increase training efficiency through initialization tricks. |
| [Sager et al., Neural Computation'26](https://doi.org/10.1162/NECO.a.1505) | The cooperative network architecture instantiates net-fragment theory; learns structured representations with strong few-shot generalisation. |

</div>
</details>


<details markdown="1">
<summary><b>Graph neural networks for pattern recognition</b></summary>
*~2022-2026: methodical deep dive*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.1145/3555776.3578600"><img src="http://stdm.github.io/images/papers/GMLR_2023.jpg" alt="GMLR 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patrec.2024.09.009"><img src="http://stdm.github.io/images/papers/PRL_2024b.jpg" alt="PRL 2024b" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/S+SSPR_2024.pdf"><img src="http://stdm.github.io/images/papers/S+SSPR_2024.jpg" alt="S+SSPR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patcog.2025.112786"><img src="http://stdm.github.io/images/papers/PR_2025.png" alt="Pattern Recognition 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/NNICE_2026.pdf"><img src="http://stdm.github.io/images/papers/NNICE_2026.jpg" alt="NNICE 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A self-contained thread, developed in collaboration with Marcello Pelillo (Venice), investigates graph-based deep learning, particularly the design of expressive yet computationally efficient *graph pooling* operators for graph classification. Key contributions include [Quasi-CliquePool](https://doi.org/10.1145/3555776.3578600) (SAC'23), [Hierarchical Glocal Attention Pooling](https://doi.org/10.1016/j.patrec.2024.09.009) (PRL'24), [Multi-View Pooling via Dominant Sets](https://doi.org/10.1016/j.patcog.2025.112786) (Pattern Recognition'26), and [Community-Hop](https://stdm.github.io/downloads/papers/S+SSPR_2024.pdf) for node classification (S+SSPR'24). These methods consistently outperform prior pooling approaches while maintaining interpretability through their graph-theoretic foundations.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Ali et al., PRL'24 *Hierarchical Glocal Attention Pooling*](https://doi.org/10.1016/j.patrec.2024.09.009) | Combining global graph structure with local neighbourhood attention in hierarchical pooling achieves state-of-the-art graph classification. |
| [Ali et al., Pattern Recognition'26 *Multi-View via Dominant Sets*](https://doi.org/10.1016/j.patcog.2025.112786) | Treating pooling as a dominant-set clustering problem provides a principled, parameter-efficient alternative to learned pooling operators. |

</div>
</details>


<details markdown="1">
<a name="speakerrec"></a>
<summary><b>Speaker recognition & audio representation learning</b></summary>

*~2004-ongoing: formative line from PhD to continued breakthroughs with deep learning*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465"><img src="http://stdm.github.io/images/papers/PhdThesis_2010.jpg" alt="PhD Thesis 2010" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ICASSP_2006.pdf"><img src="http://stdm.github.io/images/papers/ICASSP_2006.jpg" alt="ICASSP 2006" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3761"><img src="http://stdm.github.io/images/papers/MLSP_2016.jpg" alt="MLSP 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3762"><img src="http://stdm.github.io/images/papers/MLSP_2017.jpg" alt="MLSP 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patrec.2024.03.016"><img src="http://stdm.github.io/images/papers/PRL_2024a.jpg" alt="PRL 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

The earliest sustained research thread centres on automatic speaker recognition. Thilo Stadelmann's [PhD thesis](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) (Marburg, 2010) introduced the *Dimension-Decoupled Gaussian Mixture Model* for coping with very short speech segments and established that improved recognition hinges at exploitng temporal cues in a voice. Later work introduced deep learning to the field: CNNs applied directly to spectrograms ([MLSP'16](https://doi.org/10.21256/zhaw-3761), >100 citations) proved competitive for both speaker identification and clustering. Subsequent work attempted to use RNNs to capture supra-segmental voice characteristics ([ANNPR'18b](https://doi.org/10.1007/978-3-319-99978-4)) and metric-learning embeddings for measuring voice similarity ([MLSP'17](https://doi.org/10.21256/zhaw-3762)). A 2024 *Pattern Recognition Letters* paper delivers a sobering counter-result: deep networks for speaker recognition [*do not yet learn supra-segmental temporal features*](https://doi.org/10.1016/j.patrec.2024.03.016), raising open questions about what these models actually learn.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [Stadelmann, PhD thesis (2010)](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) | Supra-segmental temporal features are key to unlocking an order of magnitude lower error rates. |
| [Lukic et al., MLSP'16](https://doi.org/10.21256/zhaw-3761) (>100 citations) | CNNs on spectrograms achieve state-of-the-art speaker ID and clustering without hand-crafted features. |
| [Stadelmann et al., ANNPR'18b](https://doi.org/10.1007/978-3-319-99978-4) | RNNs seem to capture supra-segmental prosodic features for improved voice clustering. |
| [Neururer et al., PRL 2024](https://doi.org/10.1016/j.patrec.2024.03.016) | DNNs for ASR learn spectral but *not* temporal features, even if they could: the models are more superficial than expected. |

</div>
</details>


<details markdown="1">
<a name="datascience"></a>
<summary><b>Data Science as a scientific discipline</b></summary>
*~2013-2022: conceptual / disciplinary foundation work*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://stdm.github.io/downloads/papers/ECSS_2013.pdf"><img src="http://stdm.github.io/images/papers/ECSS_2013.jpg" alt="ECSS 2013" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3759"><img src="http://stdm.github.io/images/papers/HMD_2014.jpg" alt="HMD 2014" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/978-3-658-11589-0_4"><img src="http://stdm.github.io/images/papers/HMD_2016.jpg" alt="HMD 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/data-science-book/"><img src="http://stdm.github.io/images/papers/ADS_2019.jpg" alt="ADS book 2019" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/downloads/papers/ADS_2019_DataScience.pdf"><img src="http://stdm.github.io/images/papers/ADS_2019_DataScience.jpg" alt="What is Data Science" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

Running parallel to empirical research is a sustained effort to define and legitimise *data science as a discipline in its own right*, based on the early involvement of the group in founding the first continental Europan [data science lab](https://www.zhaw.ch/en/topics/interdisciplinary-competence-centres/datalab) and the corresponding [conference series](https://dblp.org/db/conf/sds2/index.html). The early papers ([ECSS'13](https://stdm.github.io/downloads/papers/ECSS_2013.pdf), [HMD'14](https://doi.org/10.21256/zhaw-3759), [HMD'16](https://doi.org/10.1007/978-3-658-11589-0_4)) characterised the emerging role of the "data scientist." The Springer edited volume [*Applied Data Science*](https://stdm.github.io/data-science-book/) (2019, >123 000 accesses) became a widely-read practitioner reference. The 2022 *Archives of Data Science* paper [*"Data Centrism and the Core of Data Science"*](https://dx.doi.org/10.5445/IR/1000143637) provides the most theoretically developed argument: that *data centrism*, treating data as the central object of study rather than a means to an end, is the overarching principle distinguishing data science from statistics, ML, and data management.

<div markdown="1">

| Paper | Key finding / message |
|---|---|
| [ECSS'13](https://stdm.github.io/downloads/papers/ECSS_2013.pdf); [HMD'14](https://doi.org/10.21256/zhaw-3759); [HMD'16](https://doi.org/10.1007/978-3-658-11589-0_4) | The data scientist profession requires a unique combination of analytics, technology, entrepreneurship, and communication; none of the contributing disciplines provides this alone. |
| [Braschler, Stadelmann, Stockinger (Eds.), Springer 2019](https://stdm.github.io/data-science-book/) (>123k accesses) | 16 case-study chapters; central lesson: "necessity is the mother of invention" - applied data science is always data-driven, not method-driven. |
| [Stadelmann, Klamt, Merkt, AoDSA'22](https://dx.doi.org/10.5445/IR/1000143637) | *Data centrism* (data as the central subject, not a resource) is the unique disciplinary core that no contributing field shares to the same degree. |

</div>
</details>



<a name="practice"></a>
## Examples of translation into practice

The table below maps concrete, practitioner-relevant examples from across the research portfolio to their domain, method, and key practical takeaways.

<style>.practice-table td { vertical-align: top; }</style>
<div class="practice-table" markdown="1">

| | Application | Domain | What was done | Practical takeaway |
|---|---|---|---|---|
| <a href="https://stdm.github.io/downloads/papers/ISBI_2026.pdf"><img src="http://stdm.github.io/images/papers/ISBI_2026.jpg" style="height:auto; width:60px;"/></a> | **Echocardiography tissue velocity measurement** | Cardiology | Automated, vendor-agnostic DL pipeline measures myocardial tissue velocities in echocardiography scans. ([ISBI'26](https://stdm.github.io/downloads/papers/ISBI_2026.pdf)) | Automating a clinically routine but tedious measurement step removes vendor lock-in and enables consistent, reproducible cardiac diagnostics. |
| <a href="https://doi.org/10.3389/frobt.2026.1764248"><img src="http://stdm.github.io/images/papers/Frontiers_2026.png" style="height:auto; width:60px;"/></a> | **AI testing infrastructure for UAVs** | Aviation / robotics | LINA testing infrastructure enables systematic AI validation in unmanned aerial vehicles, addressing certification challenges. ([Frontiers in Robotics and AI'26](https://doi.org/10.3389/frobt.2026.1764248)) | Safety-critical AI needs dedicated testing infrastructure before deployment; certification pipelines for autonomous systems must be part of the engineering process. |
| <a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" style="height:auto; width:60px;"/></a> | **AI risk assessment for public policy** | Governance / regulation | Evidence-based framework mapping technical ML properties (stochasticity, distributional shift) to policy-relevant risk categories. ([PMM'26](https://doi.org/10.1080/09540962.2025.2541304); [AI&Ethics'26](https://link.springer.com/article/10.1007/s43681-026-01042-1)) | Regulators need technically grounded criteria; the stochastic nature of ML training must be explicitly acknowledged in safety cases and hypothetical risk not overestimated. |
| <a href="https://link.springer.com/article/10.1007/s00501-025-01563-y"><img src="http://stdm.github.io/images/papers/BHM_2025.jpg" style="height:auto; width:60px;"/></a> | **3D metal printing cost optimisation** | Additive manufacturing | Merged GD&T information back from 2D engineering drawings into the 3D master model for optimised cost calculation in parts manufacturing ([BHM'25](https://link.springer.com/article/10.1007/s00501-025-01563-y)) | Data-driven cost modelling directly integrates with CAD design workflows, enabling earlier economic feasibility checks for additive manufacturing. |
| <a href="https://doi.org/10.1016/j.isci.2025.113400"><img src="http://stdm.github.io/images/papers/iScience_2025.png" style="height:auto; width:60px;"/></a> | **Human-AI teaming in safety-critical infrastructure** | Operations / safety | Systematic analysis of human-AI collaboration in safety-critical systems, introducing co-learning as a development paradigm. ([iScience'25](https://doi.org/10.1016/j.isci.2025.113400)) | Purely autonomous AI is inappropriate in regulated contexts; trust calibration, explainability, and explicit workload allocation are design requirements, not afterthoughts. |
| <a href="https://doi.org/10.1109/SDS66131.2025.00022"><img src="http://stdm.github.io/images/papers/SDS_2025a.jpg" style="height:auto; width:60px;"/></a> | **Injection moulding process monitoring & control** | Manufacturing / plastics | Representation learning for automated process monitoring ([SDS'24c](https://doi.org/10.1109/SDS60720.2024.00027)); world-model-based learning for closed-loop industrial process control from limited real data ([SDS'25a](https://doi.org/10.1109/SDS66131.2025.00022)). | Data-centric anomaly detection and world models together enable process control with very limited labelled data, showing a practical path to AI adoption in traditional manufacturing. |
| <a href="https://doi.org/10.1038/s41598-024-64855-2"><img src="http://stdm.github.io/images/papers/SR_2024.jpg" style="height:auto; width:60px;"/></a> | **Thyroid cancer cytology** | Pathology / oncology | Cell segmentation on rapid optical cytopathology images (no sending to a lab required) enables real-time diagnosis at the primary point of care. ([Sci. Reports'24](https://doi.org/10.1038/s41598-024-64855-2)) | Rapid optical biopsy becomes clinically feasible; DL cell segmentation matches standard pathology accuracy. |
| <a href="https://doi.org/10.1016/j.geothermics.2024.103012"><img src="http://stdm.github.io/images/papers/Geothermics_2024.jpg" style="height:auto; width:60px;"/></a> | **Geothermal reservoir modelling** | Energy / geology | Ensemble deep learning quantifies uncertainty in geothermal reservoir properties from sparse borehole data. ([Geothermics'24](https://doi.org/10.1016/j.geothermics.2024.103012)) | Probabilistic DL models provide actionable uncertainty bounds for drilling decisions with very limited training data. |
| <a href="https://doi.org/10.1007/978-3-031-71602-7_27"><img src="http://stdm.github.io/images/papers/ANNPR_2024.jpg" style="height:auto; width:60px;"/></a> | **Building energy optimisation** | Energy / smart buildings | RL agent controls HVAC to minimise energy consumption while satisfying occupant comfort constraints, trained in simulation. ([ANNPR'24](https://doi.org/10.1007/978-3-031-71602-7_27)) | Simulation-to-real transfer is feasible with proper domain randomisation; RL substantially outperforms rule-based controllers. |
| <a href="https://doi.org/10.5334/tismir.157"><img src="http://stdm.github.io/images/papers/TISMIR_2023.jpg" style="height:auto; width:60px;"/></a> | **Optical music recognition on real historical scores** | Cultural heritage / publishing | Deployed DL-based OMR on digitised manuscripts with domain adaptation and automated confidence scoring. ([TISMIR'24](https://doi.org/10.5334/tismir.157)) | Production OMR requires domain adaptation; benchmark accuracy on rendered scores does not predict real-world performance. |
| <a href="https://doi.org/10.1109/SDS60720.2024.00036"><img src="http://stdm.github.io/images/papers/SDS_2024b.jpg" style="height:auto; width:60px;"/></a> | **Private LLM deployment benchmark** | Enterprise IT / data privacy | Survey and benchmark of efficient on-premise LLM methods, covering quantisation, LoRA, and knowledge distillation. ([SDS'24b](https://doi.org/10.1109/SDS60720.2024.00036), *Honourable Mention Best Paper*) | Organisations can deploy capable LLMs on local hardware at acceptable quality loss; quantisation is the dominant cost-reduction lever. |
| <a href="https://doi.org/10.1002/mp.16405"><img src="http://stdm.github.io/images/papers/MedPhys_2023.jpg" style="height:auto; width:60px;"/></a> | **Radiotherapy CBCT artefact correction** | Medical physics | Deep CNNs reduce motion artefacts in cone-beam CT scans, improving image quality for treatment planning. ([MedPhys'23](https://doi.org/10.1002/mp.16405), *Top-Viewed*) | DL replaces iterative reconstruction, cutting processing from hours to seconds at equivalent image quality. |
| <a href="https://doi.org/10.1063/5.0139707"><img src="http://stdm.github.io/images/papers/APLML_2023.jpg" style="height:auto; width:60px;"/></a> | **Solar cell characterisation** | Materials / clean energy | Deep ensemble inverse models estimate physical material parameters of organic solar cells from electroluminescence images. ([APLML'23](https://doi.org/10.1063/5.0139707); [SDS'21b](https://stdm.github.io/downloads/papers/SDS_2021b.pdf), *Best Paper*) | Ensembles trained on synthetic simulation data reliably invert physical imaging models; uncertainty quantification is essential. |
| <a href="https://dx.doi.org/10.1109/ACCESS.2024.3404834"><img src="http://stdm.github.io/images/papers/Access_2024.jpg" style="height:auto; width:60px;"/></a> | **Mathematical formula recognition** | Publishing / accessibility | Data-centric approach with the FormulaNet benchmark achieves reliable printed formula detection and recognition. ([Access'22](https://doi.org/10.1109/ACCESS.2022.3202639); [Access'24](https://dx.doi.org/10.1109/ACCESS.2024.3404834)) | Data quality and annotation consistency matter more than model architecture; the bottleneck is the training set, not the network. |
| <a href="https://doi.org/10.3390/jimaging8080222"><img src="http://stdm.github.io/images/papers/JImaging_2022.jpg" style="height:auto; width:60px;"/></a> | **Vertebra detection across scanner vendors** | Radiology | Unsupervised domain adaptation with a "domain sanity loss" detects vertebrae across heterogeneous CT scanners without paired training data. ([J. Imaging'22](https://doi.org/10.3390/jimaging8080222)) | Vendor-agnostic medical AI is achievable without costly re-annotation; the domain sanity loss provides a lightweight supervision signal, needing only a handful of internal samples. |
| <a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" style="height:auto; width:60px;"/></a> | **Bias testing in face recognition** | Ethics / HR / law enforcement | Empirically tested whether "blinding" a face recognition model to gender/race reduces accuracy disparity across demographic groups. ([AI&Ethics'21](https://doi.org/10.1007/s43681-021-00108-6)) | Blinding does *not* reduce bias. Organisations cannot rely on simple attribute removal as a fairness guarantee. |
| <a href="https://doi.org/10.3390/educsci11070318"><img src="http://stdm.github.io/images/papers/EducSci_2021.jpg" style="height:auto; width:60px;"/></a> | **AI/ML teaching concept (ATLAS)** | Higher education | The AI Atlas didactic framework structures AI/ML teaching for on-site, online, and hybrid delivery, empirically validated. ([EducSci'21](https://doi.org/10.3390/educsci11070318)) | The ATLAS framework is directly transferable across institutions, offers sample syllabi and exercises, and provides educational design scaffolding. |
| <a href="https://stdm.github.io/downloads/papers/SDS_2020.pdf"><img src="http://stdm.github.io/images/papers/SDS_2020.jpg" style="height:auto; width:60px;"/></a> | **Train rescheduling** | Rail / logistics | Multi-agent RL agents reschedule delayed trains, collaborating via communication to restore timetable adherence. ([SDS'20](https://stdm.github.io/downloads/papers/SDS_2020.pdf), *Best Poster*) | RL outperforms rule-based schedulers; sample efficiency and learned communication are the bottlenecks for real deployment. |
| <a href="https://doi.org/10.1007/978-3-319-99978-4"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" style="height:auto; width:60px;"/></a> | **Face-ID verification product** | Identity & security | Full production pipeline: orientation detection, image quality assessment, anti-spoofing (3-method ensemble), face matching, user guidance. ([ANNPR'18d](https://doi.org/10.1007/978-3-319-99978-4)) | A single ML model is often not enough in production; wrapping in auxiliary quality and security modules is mandatory. |
| <a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" style="height:auto; width:60px;"/></a> | **Newspaper article segmentation** | Media / publishing | FCNNs segment printed newspaper pages into articles at >10'000 pages/day for a media monitoring company. ([ICDAR'17](https://doi.org/10.21256/zhaw-1533)) | Excluding non-article regions and handling layout diversity are the dominant engineering challenges, not the core model. |

</div>


<a name="contributions"></a>
## Main scientific contributions

The following contributions represent the group's most coherent and strong scientific claims with a clear arc, a body of evidence, and an open trajectory.


<details markdown="1">
<summary><b>Neural speaker recognition and diarization</b></summary>
*~2004-ongoing: temporal features as key, with ongoing relevance as a methodological platform*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://stdm.github.io/downloads/papers/ICASSP_2006.pdf"><img src="http://stdm.github.io/images/papers/ICASSP_2006.jpg" alt="ICASSP 2006" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3761"><img src="http://stdm.github.io/images/papers/MLSP_2016.jpg" alt="MLSP 2016" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3762"><img src="http://stdm.github.io/images/papers/MLSP_2017.jpg" alt="MLSP 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patrec.2024.03.016"><img src="http://stdm.github.io/images/papers/PRL_2024a.jpg" alt="PRL 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

Starting from first principles in signal processing and statistical modelling, this line of work built a comprehensive account of how to identify and cluster speakers automatically from audio (the task known as speaker diarization). The early contributions ([ICASSP'06](https://stdm.github.io/downloads/papers/ICASSP_2006.pdf)) introduced fast and robust speaker clustering using Earth Mover's Distance and MixMax models, operating on real-world degraded recordings without prior knowledge of the number of speakers. The [doctoral dissertation (2010)](https://archiv.ub.uni-marburg.de/ubfind/Record/urn:nbn:de:hebis:04-z2010-0465) provided the most complete treatment of voice modelling methods for speaker recognition of its time, systematically comparing generative and discriminative approaches across diverse corpora. It established the [main finding](https://doi.org/10.1145/1631272.1631300) that for speaker recognition accuracy under adverse conditions (small and noisy segments) that is on par with humans, temporal features need to be taken into account (next to spectral features).

The line was continued by deep learning, based on the hope that treating spectrograms as images would naturally allow leared features to extend into both the temporal ans spectral dimension: [MLSP'16](https://doi.org/10.21256/zhaw-3761) demonstrated that convolutional networks trained on spectrograms could learn speaker-discriminative embeddings that cluster across unseen recordings without retraining: one of the early demonstrations of this paradigm before x-vectors became standard practice. The follow-up [MLSP'17](https://doi.org/10.21256/zhaw-3762) refined the approach through metric learning objectives directly optimised for clustering quality. The 2024 [PRL article](https://doi.org/10.1016/j.patrec.2024.03.016) shows empirically that this search for methodology that adequately exploits temporal features is not over, yet. Together, this body of work documents a full methodological cycle from classical statistical approaches to neural representations, establishing the group as a European reference point in audio-based biometric intelligence.
</details>


<details markdown="1">
<summary><b>Dense small-object detection: DeepScores and the Deep Watershed Detector</b></summary>
*~2017-2025: OMR transformed, with DeepScores as an ongoing community resource*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.21256/zhaw-1533"><img src="http://stdm.github.io/images/papers/ICDAR_2017.jpg" alt="ICDAR 2017" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-4255"><img src="http://stdm.github.io/images/papers/ICPR_2018a.jpg" alt="ICPR 2018 – DeepScores" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3760"><img src="http://stdm.github.io/images/papers/ISMIR_2018.jpg" alt="ISMIR 2018 – DWD" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.5334/tismir.157"><img src="http://stdm.github.io/images/papers/TISMIR_2023.jpg" alt="TISMIR 2024" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1016/j.patcog.2025.112786"><img src="http://stdm.github.io/images/papers/PR_2025.png" alt="Pattern Recognition 2025" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

This is the group's strongest claim to a core computer vision contribution. Standard object detectors like YOLO, SSD, and Faster R-CNN share a structural failure mode when applied to images containing large numbers of very small, densely packed objects: grid-based anchor mechanisms impose spatial constraints that prevent detecting multiple co-located objects regardless of training data or hyperparameter tuning. [DeepScores (ICPR'18)](https://doi.org/10.21256/zhaw-4255), with 80 million labelled objects across 300,000 high-resolution images of music notation, makes this failure mode precisely measurable. At several orders of magnitude larger in object count than PASCAL VOC or MS-COCO, it poses the dense small-object detection problem to the broader computer vision community rather than to optical music recognition alone.

The [Deep Watershed Detector (ISMIR'18)](https://doi.org/10.21256/zhaw-3760) addresses this structurally: instead of bounding-box regression from a spatial grid, it predicts a dense energy map where object centres appear as local peaks extracted by the watershed transform. This makes it conceptually an anchor-free dense detector, contemporaneous with CornerNet (ECCV'18) but derived from different mathematical foundations that provide a clean topological justification for handling crowded scenes. A model trained on synthetically rendered scores generalised directly to handwritten notation (MUSCIMA++) without retraining, a strong out-of-distribution result. Subsequent work ([TISMIR'24](https://doi.org/10.5334/tismir.157)) extended and validated the approach on real-world scores and real-world applications, closing the translational research loop.
</details>


<details markdown="1">
<summary><b>Applied deep learning: from benchmarks to production</b></summary>
*~2018-ongoing: systematic methodology for closing the benchmark-to-deployment gap*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.1007/978-3-319-99978-4_2"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" alt="DL in the Wild" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/978-3-030-11821-1_12"><img src="http://stdm.github.io/images/papers/ADS_2019.jpg" alt="Beyond ImageNet" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://www.mdpi.com/2673-2688/1/4/31"><img src="http://stdm.github.io/images/papers/AI_2020.jpg" alt="Design Patterns 2020" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.3389/fcomp.2022.1041703"><img src="http://stdm.github.io/images/papers/Frontiers_2022.jpg" alt="Frontiers 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

A sustained and distinctive contribution addresses a problem that most ML research sidesteps: the systematic mismatch between benchmark conditions and real-world deployment. The invited position paper [*"Deep Learning in the Wild"* (ANNPR'18)](https://doi.org/10.1007/978-3-319-99978-4_2) distilled lessons from six production deployments (face verification, media monitoring, industrial quality control, music scanning, game playing, and automated machine learning) into a taxonomy of failure modes that predates much of the later "reproducibility crisis" literature in ML. Its central claim: a core DL model alone rarely suffices; reliable production systems require a surrounding ensemble of quality-assessment, uncertainty-quantification, and domain-adaptation modules to make them sample-efficient. The complementary chapter [*"Beyond ImageNet"*](https://doi.org/10.1007/978-3-030-11821-1_12) (Springer Applied Data Science book, 2019) generalises these observations into transferable design principles for practitioners who cannot assume ImageNet-like data abundance or curation.

The methodological arc culminates in two convergent results. The MDPI AI paper [*"Design Patterns for Resource-Constrained Automated Deep-Learning Methods"*](https://www.mdpi.com/2673-2688/1/4/31) (2020) synthesises the recurring architectural decisions across AutoML deployments into seven reusable patterns: a vocabulary that practitioners can apply without rediscovering the same engineering lessons from scratch. The [Frontiers in Computer Science paper (2022)](https://doi.org/10.3389/fcomp.2022.1041703) then closes the empirical loop: systematic experiments demonstrate that CNN architectures optimised on ImageNet fail to reliably transfer across domains, making the case for domain-aware architecture search. Together, this body of work constitutes a principled engineering science of deep learning deployment; not a critique of DL, but a programme for making DL efficient and robust in contexts it was not designed for.
</details>


<details markdown="1">
<summary><b>Data science as a scientific discipline</b></summary>
*~2013-2022: disciplinary foundations and the data-centrism argument*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://stdm.github.io/downloads/papers/ECSS_2013.pdf"><img src="http://stdm.github.io/images/papers/ECSS_2013.jpg" alt="ECSS 2013" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.21256/zhaw-3759"><img src="http://stdm.github.io/images/papers/HMD_2014.jpg" alt="HMD 2014" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://stdm.github.io/data-science-book/"><img src="http://stdm.github.io/images/papers/ADS_2019.jpg" alt="Applied Data Science book" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://dx.doi.org/10.5445/IR/1000143637"><img src="http://stdm.github.io/images/papers/AoDSA_2022a.jpg" alt="Data Centrism 2022" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

Running parallel to the empirical research record and influenced by leading the organizational build-up of the data science ecosystem in Switzerland (spear-heading the [first academic unit](https://www.zhaw.ch/en/topics/interdisciplinary-competence-centres/datalab) in continental Europe, the first [conference series](https://dblp.org/db/conf/sds2/index.html), and a [national association](https://data-innovation.org/) for academics and professionals) is a sustained effort to answer a question that most ML groups leave implicit: what *is* data science, and what epistemic status do its results have? The early position papers ([ECSS'13](https://stdm.github.io/downloads/papers/ECSS_2013.pdf); [HMD'14](https://doi.org/10.21256/zhaw-3759); [HMD'16](https://doi.org/10.1007/978-3-658-11589-0_4)) characterised the emerging data scientist role as requiring a combination of analytical, technological, entrepreneurial, and communicative competencies that no existing discipline provides intact, an argument against treating data science as merely applied statistics or software engineering. The Springer edited volume [*Applied Data Science*](https://doi.org/10.1007/978-3-030-11821-1) (2019, >123 000 chapter accesses) translated this argument into a practitioner reference structured around the principle that data science is always data-driven, not method-driven.

The theoretical culmination is the *Archives of Data Science* paper [*"Data Centrism and the Core of Data Science"*](https://dx.doi.org/10.5445/IR/1000143637) (AoDSA'22). Its central argument is that *data centrism* (treating data as the primary object of scientific study rather than as a resource from which models are extracted) is the unique disciplinary commitment that distinguishes data science from statistics, machine learning, and data management. Where statistics asks "what does the data tell us about the world?", data centrism asks "what is the structure of this data, and what data would allow us to answer our question?" The implication is direct: data science should evaluate its own contributions primarily by the datasets it produces, curates, and analyses, not only by model accuracy on fixed benchmarks. This reframes the reproducibility discussion and provides a philosophically grounded rationale for why dataset creation and work on novel use cases counts as first-class scientific work.
</details>


<details markdown="1">
<summary><b>From algorithmic research to societal questions</b></summary>
*~2018-ongoing: increasingly the intellectual orientation based on the algorithmic expertise*

<div style="display:flex; flex-wrap:wrap; gap:8px; margin:0.8em 0 1em; justify-content:center;">
<a href="https://doi.org/10.1007/978-3-319-99978-4_2"><img src="http://stdm.github.io/images/papers/ANNPR_2018d.jpg" alt="Deep Learning in the Wild" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-021-00108-6"><img src="http://stdm.github.io/images/papers/AIEthics_2021.jpg" alt="AI Ethics 2021" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-023-00408-z"><img src="http://stdm.github.io/images/papers/AIEthics_2023.jpg" alt="AI Ethics 2023" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1080/09540962.2025.2541304"><img src="http://stdm.github.io/images/papers/PMM_2025.png" alt="PMM 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
<a href="https://doi.org/10.1007/s43681-026-01042-1"><img src="http://stdm.github.io/images/papers/AIEthics_2026.jpg" alt="AI Ethics 2026" style="height:120px; width:auto; border:1px solid #c8d8ea; border-radius:3px;"/></a>
</div>

The group has systematically traced what happens when machine learning results exit the research lab and encounter real human contexts, producing original scientific arguments at each stage of that transition. The invited position paper [Deep Learning in the Wild (ANNPR'18)](https://doi.org/10.1007/978-3-319-99978-4_2) opened this line by cataloguing the gap between benchmark conditions and deployment realities, providing a taxonomy of failure modes that predates much of the later "reproducibility crisis" literature in ML. These were translated for non-technical audiences in a [2019 invited chapter](https://stdm.github.io/downloads/papers/FCW_2019.pdf) that aged quite well with respect to its recommendations concerning the following 5 years. 

On the applied side, the [AI and Ethics (2021)](https://doi.org/10.1007/s43681-021-00108-6) bias study showed quantitatively that demographic awareness in face recognition design does not translate to reduced bias at deployment. [Assessing Deep Learning (AI and Ethics'23)](https://doi.org/10.1007/s43681-023-00408-z) proposed a humanities-grounded framework for evaluating AI systems beyond technical metrics. Most recently, [PMM'26](https://doi.org/10.1080/09540962.2025.2541304) and [AI and Ethics'26](https://doi.org/10.1007/s43681-026-01042-1) formalised how intrinsic ML properties (stochasticity of training, distributional shift) map to policy-relevant risk categories, giving regulators technically grounded criteria that go beyond checklist compliance. In another translatory effort, these have been made accessible to general public audiences in form of a [TEDx talk](https://youtu.be/deVbP-hViMQ).
</details>                                                                                  


<a name="ideas"></a>
## Ideas we'd love to work on in the future

Project opportunities abound, and we are involved in several activities in medical imaging, multimedia analysis, robotics / physical AI, speaker diarization (to name a few). However, the following 5 research directions that emerged from our work appear to us as "golden": ideas that have not yet reached full maturity, yet their potential impact can already now be assessed as huge. Hence, we are actively seeking ways to inquire more in these directions and seek respective collaborations, notwithstanding our general openness to interesting use cases and challenges. The order is from algorithmic to societal, the links point to previous publications giving more insight. If you are interested in those (and see an opportunity also for funding respective work), please get in touch.

  * [Next-level, neuroscience-informed AI](https://arxiv.org/abs/2205.00002) based on **world models** for higher sample efficiency and robust understanding of cause and effect of actions
  
  * Towards **document foundation models** based on an understanding of [document recognition as image-to-record transcription](https://arxiv.org/abs/2507.08458)
  
  * **Co-learning** as a [framework for human-AI teaming](https://doi.org/10.1007/s43681-026-01042-1) in high-consequence environments
  
  * **Pro-human AI design** as a [methodology to build AI systems](https://stdm.github.io/Pro-human-AI/) specifically with the individual human's flourishing in mind (instead of accidentally eroding the human's core)
  
  * **Scenario development** for [positive visions](https://stdm.github.io/AI-in-2035/) for our societal future with AI
