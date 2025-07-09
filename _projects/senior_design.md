---
layout: page
title: Four‑Axis Vacuum Stage for Advanced Nano‑Manufacturing
description: A four‑degree‑of‑freedom robotic vacuum stage for uniform 3D nanocoating of irregular objects, designed to operate inside a magnetron sputtering chamber with high precision and reliability.
img: assets/img/projects/senior_design/overview.png
importance: 2
category: Hardware & Systems
github: https://github.com/Yonghonghui/Four-Axis-Vacuum-Stage
---

## Overview

We designed and fabricated a **Four‑Axis Vacuum Stage**, a 4‑DOF aluminum robotic arm integrated directly into a magnetron sputtering chamber. It enables conformal nanocoating on both flat and complex 3D substrates under high‑vacuum and elevated temperatures, overcoming the uniformity challenges of traditional 2D frame processes.

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold">GitHub Repository</h5>
    <a href="https://github.com/Yonghonghui/Four-Axis-Vacuum-Stage" target="_blank">
      <i class="fab fa-github"></i> Four‑Axis Vacuum Stage Code & Schematics
    </a>
  </div>
</div>

## Project Implementation & Demo

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/sputtering_machine.png" title="Magnetron Sputtering Chamber" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  High‑vacuum magnetron sputtering chamber used for uniform nanocoating experiments, with viewports for real‑time process monitoring.
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/robotic_arm.jpg" title="V2 Robotic Arm Prototype" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Second‑generation aluminum arm with screw‑drive and electromagnetic brake, ready for vacuum integration.
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/stm32board.jpg" title="STM32F407 Control Board" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Custom STM32F407‑based control board handling motion commands, RS‑485 communication, and HMI interface signals.
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/pcb.jpg" title="Power & Signal Distribution PCB" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/motor_drivers.jpg" title="Emm42 Stepper Motor Drivers" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Left: Custom PCB with optical isolators and 24 V power routing for noise‑free operation. Right: Four Emm42 stepper drivers on DIN rail, providing precise open‑loop control via RS‑485.
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/senior_design/tftscreen.jpg" title="7″ TFT Touchscreen Interface" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  User interface displaying preset motion routines, real‑time arm position, and emergency‑stop controls for safe operation.
</div>


## Technical Details

- **Mechanical Design**  
  - 4‑DOF arm built from vacuum‑compatible aluminum and 2020 extrusions  
  - Screw‑motor drive on Joint 2 for high torque and self‑locking  
  - Integrated electromagnetic brake for power‑loss safety  
- **Control System**  
  - STM32F407 MCU with RS‑485 bus to four Emm42 stepper drivers  
  - Custom PCB distributes 24 V and isolates noise via optical couplers  
  - Open‑loop motion with periodic status polling and TFT touchscreen UI  
- **Nanocoating Experiments**  
  - Uniform 900 nm Cr film on flat substrate at 300 mA, 0.5 h, 300 °C  
  - Conformal coverage on a rotating 3D brass cylinder, demonstrating 3D capability  

## Key Features

- High‑precision 4‑axis manipulation in vacuum  
- Uniform 3D nanocoating for irregular geometries  
- Industrial‑grade RS‑485 communication and optical isolation  
- Modular aluminum construction for cost‑effective fabrication  
- User interface with preset motion routines and emergency stop

## Technical Stack

PCB Layout (KiCad) · STM32 MCU · RS‑485 · Emm42 Steppers · Fusion 360 & FEA · Magnetron Sputtering

## Project Advisor

Prof. Oleskiy Penkov, Zhejiang University

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include video.liquid path="assets/video/projects/senior_design/demo.mp4" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Video demo: Automated chromium sputtering on a 3D brass cylinder (right-click to play).
</div>
