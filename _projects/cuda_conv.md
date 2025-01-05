---
layout: page
title: CUDA Optimized CNN
description: Implemented and optimized convolutional neural networks using CUDA for high-performance computing
# img: assets/img/projects/cuda.jpg
importance: 1
category: Hardware & Systems
---

## Overview

Designed and implemented a highly optimized CUDA-based convolutional neural network, focusing on the forward pass of convolutional layers for a modified LeNet-5 architecture. The project aimed to achieve maximum performance for deep learning tasks such as image classification and object detection.

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
Prof. Yao Chen, Zhejiang University 