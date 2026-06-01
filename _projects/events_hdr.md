---
layout: paper-project
title: Event-based HDR
description: Project page for "HDR Reconstruction from Bracketed Exposures and Events"
img: assets/img/eventhdr22/figure1.png
importance: 4
category: paper
---

<center>

<h2><b>HDR Reconstruction from Bracketed Exposures and Events</b></h2>
<h5>BMVC 2022</h5>
               
<br>

<a href="https://scholar.google.com/citations?user=9qqtzK4AAAAJ&hl=en">Richard Shaw</a>
&nbsp;&nbsp;
<a href="https://sib1.github.io/">Sibi Catley-Chandar</a>
&nbsp;&nbsp;
<a href="https://scholar.google.com/citations?user=BEFl4j0AAAAJ&hl=en">Aleš Leonardis</a>
&nbsp;&nbsp;
<a href="https://perezpellitero.github.io/">Eduardo Pérez-Pellitero</a>

<br>
Huawei Noah’s Ark Lab
<br><br>

<div class="row links-list justify-content-center">
    
    <div class="col-auto mt-3 mt-md-0">
    	<a href="https://arxiv.org/abs/2203.14825">
        <img  src="{{'/assets/img/eventhdr22/paper-thumb.png'}}" height="150px" alt="paper" title="arXiv"/>
        <br><p>ArXiv</p>
        </a>
    </div>

    <div class="col-auto mt-3 mt-md-0">
    	<a href="https://bmvc2022.mpi-inf.mpg.de/0603_poster.pdf">
        <img src="/assets/img/eventhdr22/poster-thumb.png" height="150px" alt="paper poster" title="Poster"/>
        <br><p>Poster</p>
        </a>
    </div>

</div>
</center>

---

#### TLDR

Multimodal camera system that uses neuromorphic (event-based) sensor together with bracketed RGB images to obtain state-of-the-art quality, surpassing methods using single sensors or bi-sensors without frame bracketing.

<div class="row mt-3">
    <div class="col-sm mt-6 mt-md-0">
        {% include figure.liquid path="assets/img/eventhdr22/figure1.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    Our learning-based method produces high-quality HDR images, leveraging bracketed LDRs and events.
</div>

#### Abstract

<p align="justify">
Reconstruction of high-quality HDR images is at the core of modern computational photography. Significant progress has been made with multi-frame HDR reconstruction methods, producing high-resolution, rich and accurate colour reconstructions with high-frequency details. However, they are still prone to fail in dynamic or largely over-exposed scenes, where frame misalignment often results in visible ghosting artifacts. Recent approaches attempt to alleviate this by utilizing an event-based camera (EBC), which measures only binary changes of illuminations. Despite their desirable high temporal resolution and dynamic range characteristics, such approaches have not outperformed traditional multi-frame reconstruction methods, mainly due to the lack of colour information and low-resolution sensors. In this paper, we propose to leverage both bracketed LDR images and simultaneously captured events to obtain the best of both worlds: high-quality RGB information from bracketed LDRs and complementary high frequency and dynamic range information from events. We present a multi-modal end-to-end learning-based HDR imaging system that fuses bracketed images and event modalities in the feature domain using attention and multi-scale spatial alignment modules. We propose a novel event-to-image feature distillation module that learns to translate event features into the image-feature space with self-supervision. Our framework exploits the higher temporal resolution of events by sub-sampling the event streams using a sliding window, enriching our combined feature representation. Our proposed approach surpasses state-of-the-art (SoTA) multi-frame HDR reconstruction methods using synthetic and real events, with a 2dB and 1dB improvement in PSNR-L and PSNR-$\mu$ on the HdM HDR dataset, respectively.
</p>

<br>

#### BibTeX Citation

```
@article{shaw2022eventhdr,
	title={HDR Reconstruction from Bracketed Exposures and Events},
	author={Richard Shaw, Sibi Catley-Chandar, Ales Leonardis and Eduardo P\'erez-Pellitero},
	journal={BMVC 2022},
	year={2022},
}
```
