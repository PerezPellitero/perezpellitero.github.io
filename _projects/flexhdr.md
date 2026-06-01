---
layout: paper-project
title: FlexHDR
description: Project page for "FlexHDR TIP paper"
img: assets/img/flexhdr/architecture.png
importance: 4
category: paper
---

<center>

<h2><b>FlexHDR: Modelling Alignment and<br>Exposure Uncertainties for Flexible HDR Imaging</b></h2>
<h5>IEEE Transactions On Image Processing 2022</h5>

<br> 

<a href="https://scholar.google.com/citations?user=RvAaCDEAAAAJ&hl=en">Sibi Catley-Chandar</a>
&nbsp;&nbsp;
<a href="https://scholar.google.com/citations?user=wCC0VK0AAAAJ&hl=en">Thomas Tanay</a>
&nbsp;&nbsp;
<a href="https://ch.linkedin.com/in/lucasvandroux">Lucas Vandroux</a>
&nbsp;&nbsp;
<a href="https://scholar.google.com/citations?user=BEFl4j0AAAAJ&hl=en">Aleš Leonardis</a>
&nbsp;&nbsp;
<a href="https://perezpellitero.github.io">Eduardo Pérez-Pellitero</a>

<br><br>
Huawei Noah’s Ark Lab <br>
Queen Mary, University of London
<br><br>


<div class="row links-list justify-content-center">

    <div class="col-auto mt-3 mt-md-0">
    	<a href="https://ieeexplore.ieee.org/document/9881970">
        <img  src="/assets/img/flexhdr/proceedings.jpg" height="120px" title="Journal"/>
        <br><p>Journal</p>
        </a>
    </div>
    
    <div class="col-auto mt-3 mt-md-0">
    	<a href="https://arxiv.org/abs/2201.02625">
        <img  src="/assets/img/flexhdr/paper.png" height="120px" title="ArXiv"/>
        <br><p>ArXiv</p>
        </a>
    </div>

     <div class="col-auto mt-3 mt-md-0">
    	<a href="https://drive.google.com/file/d/1LjtDcuxtkZs8dmHoCsiPmLrzi4dD57j6/view">
        <img  src="/assets/img/flexhdr/results.jpg" height="120px" alt="results" title="Results"/>
        <br><p>Image Results</p>
        </a>
    </div>
    
</div>
      
</center>
----
#### Abstract

<p align="justify">
High dynamic range (HDR) imaging is of fundamental importance in modern digital photography pipelines and used to produce a high-quality photograph with well exposed regions despite varying illumination across the image. This is typically achieved by merging multiple low dynamic range (LDR) images taken at different exposures. However, over-exposed regions and misalignment errors due to poorly compensated motion result in artefacts such as ghosting. In this paper, we present a new HDR imaging technique that specifically <b>models alignment and exposure uncertainties</b> to produce high quality HDR results. We introduce a strategy that learns to jointly align and assess the alignment and exposure reliability using an HDR-aware, uncertainty-driven attention map that robustly merges the frames into a single high quality HDR image. Further, we introduce a progressive, multi-stage image fusion approach that can <b>flexibly merge any number of LDR images in a permutation-invariant manner</b>. Experimental results show our method can produce better quality HDR images with <b>up to 1.1dB PSNR improvement to the state-of-the-art</b>, and subjective improvements in terms of better detail, colours, and fewer artefacts.
</p>

#### Overview

<center>
<img class="img-fluid rounded z-depth-1 medium-zoom-image" src="/assets/img/flexhdr/architecture.png" data-zoomable="" style="max-width: 100%;" alt="flexhdr model architecture">
</center>
<div class="caption">Our model architecture consists of a HDR flow network, uncertinaty aware attention and multi-stage fusion. Our model accepts any number of LDR images as input.
</div>
<br>


#### Results

<center>
    <figure class="col-md-8 col-md-offset-2">
    <img src="/assets/img/flexhdr/fireplace_tursun.png" class="img-responsive"  
     style="max-width: 100%;" alt="flexhdr results tursun">
        <figcaption>
        Our model can utilize information from all 9 input frames, despite having only seen 3 input frames during training.
        </figcaption>
    </figure>
</center>

<center>
    <figure class="col-md-8 col-md-offset-2">
    <img src="/assets/img/flexhdr/results_kalantari.png" class="img-responsive"  
     style="max-width: 100%;" alt="flexhdr results kalantari">
        <figcaption>
        Results on an image from the Kalantari test set. 
        </figcaption>
    </figure>
</center>

<center>
    <figure class="col-md-8 col-md-offset-2">
    <img src="/assets/img/flexhdr/reference_frames.png" class="img-responsive"  
     style="max-width: 100%;" alt="flexhdr reference frame">
        <figcaption>
        LDR reference frame (top) and HDR reconstruction (bottom). Our method accepts any frame as the reference frame without re-training.
        </figcaption>
    </figure>
</center>

#### BibTeX Citation

```
@article{catleychandar2022,
  author={Catley-Chandar, Sibi and Tanay, Thomas and Vandroux, Lucas and Leonardis, Ales and Slabaugh, Gregory and P\'erez-Pellitero, Eduardo},
  journal={IEEE Transactions on Image Processing}, 
  title={Flex{HDR}: Modeling Alignment and Exposure Uncertainties for Flexible {HDR} Imaging}, 
  year={2022},
  volume={31},
  }
```