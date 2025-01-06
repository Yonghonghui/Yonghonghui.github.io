---
layout: page
title: Over-the-Air-Computation Based Federated Learning
description: Established and simulated Over-the-Air computation based federated learning model using MATLAB/Simulink
importance: 1
category: Machine Learning & Communications
---

## Overview

Developed a novel approach to federated learning using Over-the-Air (OTA) computation, implementing both basic AM modulation and advanced OFDM-based communication architectures in MATLAB/Simulink.

## Theoretical Framework

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/over_the_air/1.png" title="OTA-FL Theory" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Theoretical framework of analog Over-the-Air computation based Federated Learning, showing the mathematical principles and system design.
</div>

## Basic Implementation

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/over_the_air/2.png" title="AM Implementation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulink implementation using basic AM modulation/demodulation with 4 local devices, demonstrating the fundamental OTA computation concept.
</div>

## OFDM-based Architecture

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/over_the_air/3.png" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/over_the_air/4.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: OFDM transmitter architecture for OTA computation. Right: OFDM receiver design with built-in synchronization and channel estimation.
</div>

## Technical Details

- Implemented two communication architectures:
  - Basic AM modulation/demodulation system
  - Advanced OFDM-based system with built-in synchronization
- Developed federated learning algorithms:
  - Distributed model training
  - Parameter aggregation via OTA computation
  - Model convergence optimization
- Conducted comprehensive simulations:
  - Channel estimation and compensation
  - Synchronization performance analysis
  - System throughput evaluation

## Key Features

- Analog Over-the-Air computation
- Multi-device parameter aggregation
- OFDM-based communication
- Channel estimation and compensation
- Distributed model training
- Real-time parameter updates

## Technical Stack

- MATLAB/Simulink
- Communication Systems
- Signal Processing
- Machine Learning
- OFDM Technology
- Channel Modeling
- System Optimization

## Project Advisor
Prof. Howard Yang