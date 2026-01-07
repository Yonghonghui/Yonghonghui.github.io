---
layout: page
title: High-Precision Fully-Differential Folded-Cascode Op-Amp
description: Low-power analog amplifier design in 180nm CMOS with continuous-time CMFB.
img: assets/img/projects/opamp/schematic.png
importance: 2
category: Analog/Digital/Mixed Integrated Circuit Design
# github: https://github.com/yourusername/project-repo
---

## Overview

Designed and optimized a fully-differential Folded-Cascode Operational Amplifier using 180nm CMOS technology. The project focused on the trade-off between power consumption and settling speed, culminating in a low-power design (2.21 mW) that drives a 2 pF capacitive load with <1% gain error and a 1.6 $V_{pp}$ output swing. The design features a robust triode-region Common-Mode Feedback (CMFB) network and systematic mismatch mitigation techniques.

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">Project Documents</h5>
    <a href="/assets/pdf/215AFinal_Project.pdf" target="_blank">
      <i class="fas fa-file-pdf"></i> Final Design Report
    </a>
  </div>
</div>

## Project Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/opamp/schematic.png" title="Folded-Cascode Schematic" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Schematic of the Low-Power (Version 2) Fully-Differential Folded-Cascode Amplifier, featuring NMOS input pairs and a passive triode-region CMFB network.
</div>

## Performance Metrics

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <div class="table-responsive">
            <table class="table table-sm table-borderless">
                <thead>
                    <tr>
                        <th scope="col">Metric</th>
                        <th scope="col">Value (Low-Power Ver.)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Technology</strong></td>
                        <td>180nm CMOS</td>
                    </tr>
                    <tr>
                        <td><strong>Supply Voltage</strong></td>
                        <td>1.8 V</td>
                    </tr>
                    <tr>
                        <td><strong>Total Power</strong></td>
                        <td>2.21 mW</td>
                    </tr>
                    <tr>
                        <td><strong>Output Swing</strong></td>
                        <td>1.6 V<sub>pp</sub> (Differential)</td>
                    </tr>
                    <tr>
                        <td><strong>Settling Time (99%)</strong></td>
                        <td>45 ns</td>
                    </tr>
                     <tr>
                        <td><strong>Gain Error</strong></td>
                        <td>< 1% (Closed-Loop Gain = 8)</td>
                    </tr>
                    <tr>
                        <td><strong>Load Capacitance</strong></td>
                        <td>2 pF</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</div>
<div class="caption">
    Performance summary for the optimized low-power design variant, satisfying all settling and accuracy requirements.
</div>

## Technical Details

- **Folded-Cascode Topology:**
<div class="row">
  <div class="col-sm-8 mt-3 mt-md-0 mx-auto">
    {% include figure.liquid path="assets/img/projects/opamp/topology_core.png" title="Core Topology" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Figure 1: NMOS-input Folded-Cascode architecture selected for high-speed operation.
</div>
  - Selected an NMOS-input folded-cascode architecture to maximize transconductance ($g_m$) and Gain-Bandwidth Product (GBW) for high-speed operation.
  - Allocated overdrive voltages ($V_{ov}$) meticulously to ensure all transistors remain in saturation while supporting a wide **1.6 $V_{pp}$ output swing**.

- **Triode-Region CMFB:**
<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0 mx-auto">
    {% include figure.liquid path="assets/img/projects/opamp/cmfb_circuit.png" title="CMFB Circuit" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Figure 2: Continuous-time CMFB utilizing triode-region transistors for zero static power.
</div>
  - Implemented a continuous-time Common-Mode Feedback network using transistors in the triode region.
  - **Advantage:** Eliminates the need for resistive dividers (saving area) and avoids consuming voltage headroom at the output nodes.

- **Settling Time Optimization:**
  - Identified a critical bottleneck where large CMFB devices introduced excessive parasitic capacitance at the output nodes.
  - **Optimization:** Reduced CMFB device sizes by **50%**, significantly lowering capacitive loading and improving the slewing / small-signal settling time without compromising stability.

- **Systematic Mismatch Mitigation:**
  - Inserted compensation resistors in the bias branches to equalize $V_{DS}$ between the current mirror reference and the main tail current source.
  - This ensures precise current mirroring ratios and robust DC operating points by mitigating Channel Length Modulation (CLM) effects

## Simulation Results

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/opamp/transient_response.png" title="Transient Settling Response" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Transient response to a 100 mV differential step input. The output settles to within 1% accuracy in approximately 45 ns.
</div>

## Technical Stack

- **EDA Tools:** Cadence Virtuoso Schematic Editor, Spectre Simulator, Virtuoso ADE
- **Process Technology:** 180nm CMOS
- **Methodology:** Analog Circuit Design, Sizing & Biasing, Parasitic Estimation, Transient/AC Analysis

## Course
UCLA EE 215A -- Analog Integrated Circuit Design (25Fall) -- Prof. Behzad Razavi