---
layout: page
title: 5 Gb/s Wireline Transmitter with Low-Jitter PLL
description: High-speed transmitter in 180nm CMOS featuring a 2.5 GHz LC-VCO and hybrid divider architecture.
img: assets/img/projects/pll/transmitter_top.png
importance: 1
category: Analog/Digital/Mixed Integrated Circuit Design
---

## Overview

Designed and optimized a complete **5 Gb/s Non-Return-to-Zero (NRZ)** wireline transmitter using 180nm CMOS technology. The architecture integrates a high-performance **Type-II, 3rd-order PLL** providing a stable 2.5 GHz clock, an **8-to-1 serializer MUX tree**, and a differential line driver. Key design focuses included flicker noise mitigation in the LC-VCO, current matching in the charge pump, and achieving high energy efficiency of **5.942 pJ/bit**.

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">Project Documents</h5>
    <a href="/assets/pdf/ECE215E_Final_Report.pdf" target="_blank">
      <i class="fas fa-file-pdf"></i> Final Project Report
    </a>
  </div>
</div>

## Project Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/pll/system_schematic.png" title="PLL Blockwise Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Complete schematic of PLL, featuring a fully integrated Type-II PLL (PFD, Charge Pump, 3rd-order Loop Filter, and LC-VCO) with a hybrid divider chain.
</div>

## Performance Metrics

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <div class="table-responsive">
            <table class="table table-sm table-borderless">
                <thead>
                    <tr>
                        <th scope="col">Metric</th>
                        <th scope="col">Value</th>
                        <th scope="col">Specification</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Technology</strong></td>
                        <td>180nm CMOS</td>
                        <td>Standard Process</td>
                    </tr>
                    <tr>
                        <td><strong>Data Rate</strong></td>
                        <td>5 Gb/s (NRZ)</td>
                        <td>≥ 5 Gb/s</td>
                    </tr>
                    <tr>
                        <td><strong>Total Power</strong></td>
                        <td>29.71 mW</td>
                        <td>Measured</td>
                    </tr>
                    <tr>
                        <td><strong>Energy Efficiency</strong></td>
                        <td>5.942 pJ/bit</td>
                        <td>Competitive</td>
                    </tr>
                    <tr>
                        <td><strong>RMS Jitter</strong></td>
                        <td>< 4 ps</td>
                        <td>≤ 4 ps</td>
                    </tr>
                    <tr>
                        <td><strong>Reference Spur</strong></td>
                        <td>-56.82 dBc</td>
                        <td>≤ -30 dBc</td>
                    </tr>
                    <tr>
                        <td><strong>Phase Noise</strong></td>
                        <td>-131.39 dBc/Hz</td>
                        <td>@ 10 MHz offset</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</div>

## Technical Details

- **Low-Noise LC-VCO Design:**
  - Implemented a cross-coupled NMOS topology with a **120 µm** width to specifically suppress **86% flicker noise** ($1/f$) contribution.
  - Optimized the LC tank with $L = 1$ nH ($Q=8$) and a combination of NMOS varactors and fixed capacitors to achieve a robust 2.5 GHz oscillation with precise tuning.

- **Hybrid Divider & Level Shifter:**
  - Utilized a high-speed **CML divide-by-2 stage** for the 2.5 GHz VCO output and a **$C^2$MOS stage** for power-efficient intermediate division.
  - A **self-biased inverter** with AC-coupling (200 fF) restores low-swing CML signals to rail-to-rail CMOS levels.

- **Current-Steering Charge Pump & LPF:**
  - Designed a current-steering CP with matched current mirrors to minimize charge injection and $V_{cont}$ ripple.
  - Integrated a **3rd-order Loop Filter** ($R_0 = 5$ kΩ, $C_1 = 12.7$ pF, $C_0 = 1.3$ pF) for stability and spur attenuation.

- **Serializer & Differential Driver:**
  - Implemented an **8-to-1 serializer tree** using $C^2$MOS logic and retiming latches to ensure timing margin at 5 Gb/s.
  - Optimized the driver for an on-resistance of **55–58 Ω** to maintain a **1.06 V** differential output swing across a 50 Ω load.

## Simulation Results

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/pll/locked_clocks.png" title="Locked Clocks" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/pll/vcont_locking.png" title="PLL Locking Profile" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    PLL Transient Analysis. Left: Synchronized multi-phase clocks (2.5/1.25/0.625 GHz). Right: Control voltage ($V_{cont}$) settling between 885 mV and 929 mV.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/pll/eye_diagram.png" title="Output Eye Diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Final 5 Gb/s differential output eye diagram, demonstrating a clear 0.9 UI opening and 1.06 V peak-to-peak differential swing.
</div>

## Technical Stack

- **EDA Tools:** Cadence Virtuoso, Spectre Simulator, ADE Explorer/Assembler
- **Design Modules:** LC-VCO, PFD/CP, LPF, CML/C2MOS Dividers, 8:1 Serializer, Line Driver
- **Methodology:** Frequency Synthesizer Design, Noise/Spur Optimization, High-Speed Link Budgeting

## Course
UCLA ECE 215E -- Mixed-Signal IC Design (26Winter) -- Prof. Behzad Razavi