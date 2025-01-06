---
layout: page
title: RRAM-based Multimodal BCI
description: Developed heterogeneous processing system for multimodal brain-computer interfaces using RRAM technology
# img: assets/img/projects/bci.jpg
importance: 1
category: BCI & Neural Computing
# github: https://github.com/YourUsername/rram-bci
---

## Overview

Developed a RRAM-based heterogeneous processing system for multimodal brain-computer interfaces, focusing on P300 signal recognition and integration with other BCI modalities.

## P300 Signal Characteristics

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/rram_bci/1.png" title="P300 Signal" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Typical P300 ERP waveform showing the characteristic positive deflection approximately 300ms after stimulus onset.
</div>

## EEGNet Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/rram_bci/2.png" title="Original EEGNet" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Original EEGNet architecture showing the temporal and spatial convolution layers for EEG signal processing.
</div>

## RRAM-based Classification

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/rram_bci/4.png" title="RRAM Classification" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    RRAM-based P300 signal classification paradigm showing the compute-in-memory approach for efficient neural processing.
</div>

## Modified Architecture

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/rram_bci/3.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/rram_bci/5.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: Modified EEGNet architecture optimized for P300 signal processing. Right: Multimodal EEG signal classification system combining P300 and MI signals using RRAM chips.
</div>

## Technical Details

- Simulated representative heterogeneous processing paradigm of P300 signal recognition using resistive random-access memory (RRAM)
- Implemented and evaluated fixed parameter disturbance training (FDT) techniques
- Combined multiple datasets:
  - BCIC IV IIa dataset
  - P300 RSVP dataset
- Designed an RRAM-based multimodal recognizer integrating:
  - Pre-trained EEGNet
  - Common Spatial Pattern (CSP)
  - Modality-fused classifier

## Results & Achievements

- Achieved 2.83% higher accuracy using multimodal BCI with FDT compared to without FDT
- Significantly outperformed single-modality approaches:
  - 8.19% improvement over MI-alone results
  - 13.20% improvement over P300-alone results

## Skills & Technologies

- Brain-Computer Interfaces
- RRAM Technology
- Signal Processing
- Machine Learning
- Python Programming
- Neural Networks

## Project Advisor
Dr. Zhengwu Liu, The University of Hong Kong 

<!-- <div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/projects/your_project/video.mp4" 
                              class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    视频说明文字
</div>  -->