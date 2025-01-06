---
layout: page
title: CUDA Optimized CNN
description: Implemented and optimized convolutional neural networks using CUDA for high-performance computing
# img: assets/img/projects/cuda.jpg
importance: 1
category: Hardware & Systems
github: https://github.com/illinois-cs-coursework/fa24_ece408_yc47/tree/9759cfd8a93af4c5496e6d7133dc5f4a1deec6ff/Project
---

## Overview

Designed and implemented a highly optimized CUDA-based convolutional neural network, focusing on the forward pass of convolutional layers for a modified LeNet-5 architecture. The project aimed to achieve maximum performance for deep learning tasks such as image classification and object detection.

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">GitHub Repository</h5>
    <a href="https://github.com/illinois-cs-coursework/fa24_ece408_yc47/tree/9759cfd8a93af4c5496e6d7133dc5f4a1deec6ff/Project" target="_blank">
      <i class="fab fa-github"></i> CUDA CNN Implementation
    </a>
  </div>
</div>

## Implementation Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/cuda_cnn/1.png" title="CUDA Implementation Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Architecture diagram showing the CUDA-based CNN implementation with memory management and computation optimization.
</div>

## Technical Details

- Implemented GPU-based forward convolution using CUDA C++ with a structured Prolog-Kernel-Epilog approach
- Ensured proper memory management, convolution computation, and output transfer
- Matched CPU implementation correctness while optimizing performance using Nsight profiling tools
- Applied advanced GPU programming techniques including:
  - CUDA streams for concurrent execution
  - GEMM kernels for matrix operations
  - Kernel fusion for reduced overhead
  - Optimized memory access patterns
  - Efficient data parallelism strategies

## Key Achievements

- Achieved target inference time of ≤80ms for 10,000 images from the Fashion MNIST dataset
- Optimized memory access patterns for improved throughput
- Implemented efficient data parallelism strategies
- Reduced computational overhead through algorithmic optimizations
- Successfully validated against CPU implementation for accuracy

## Technical Stack

- CUDA C++
- Parallel Programming
- GPU Computing
- Performance Optimization
- Deep Learning
- Computer Vision
- Convolutional Neural Networks
- Nsight Profiling Tools

## Project Advisor
Prof. Volodymyr Kindratenko, UIUC