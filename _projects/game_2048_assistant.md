---
layout: page
title: 2048 Game Assistant
description: Developed an Android app that analyzes live 2048 game state and suggests optimal moves
importance: 3
category: Machine Learning
github: https://github.com/Yonghonghui/ECE420-Final-Project
---

## Overview

Created an intelligent assistant for the game 2048 that combines real-time image processing with AI decision-making to analyze the game state and recommend optimal moves.

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">GitHub Repository</h5>
    <a href="https://github.com/Yonghonghui/ECE420-Final-Project" target="_blank">
      <i class="fab fa-github"></i> 2048 Game Assistant
    </a>
  </div>
</div>

## System Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/game_2048/1.jpg" title="System Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    System architecture diagram showing the image processing pipeline and AI decision-making process.
</div>

## Technical Details

- Implemented advanced image processing pipeline:
  - Grayscale conversion
  - Canny edge detection
  - Perspective transformation
  - Template matching for digit recognition
- Developed AI decision engine:
  - Expecti-max Search algorithm
  - Corner placement strategy
  - Move evaluation heuristics
- Built Android application:
  - Real-time camera feed processing
  - Game state analysis
  - Move recommendation display

## Key Achievements

- 100% digit recognition accuracy with proper alignment
- Consistent AI performance reaching 1024 tile in 75% of simulations
- Real-time processing and move suggestion
- Robust board state detection
- Efficient template matching system

## Technical Stack

- Android Studio
- Java/Kotlin
- OpenCV
- Image Processing
- Machine Learning
- Real-time Systems
- Mobile Development
- Computer Vision

## Project Advisor
Prof. Thomas Moon, UIUC 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/projects/game_2048/1.mp4" 
                              class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Demo of our ECE420 Final Porject -- "Game 2048 Cheat Machine" (Right click on the cover above to view the video)
</div> 