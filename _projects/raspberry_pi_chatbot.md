---
layout: page
title: IoT Private Chatbot
description: Developed a Raspberry Pi based IoT system as a private chatbot with face and speaker recognition
importance: 2
category: Machine Learning
github: https://github.com/Yonghonghui/ECE479-raspberry-pi4
---

## Overview

Developed an IoT system using Raspberry Pi 4 as a private chatbot with face detection and speaker recognition to guarantee privacy and personal conversations as well as interactions.

## System Architecture

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/raspi_iot/1.png" title="System Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    System architecture showing the integration of face recognition, speech processing, and AI assistant components on Raspberry Pi 4.
</div>

## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">GitHub Repository</h5>
    <a href="https://github.com/Yonghonghui/ECE479-raspberry-pi4" target="_blank">
      <i class="fab fa-github"></i> Raspberry Pi Smart Assistant
    </a>
  </div>
</div>

## Technical Details

- Implemented MTCNN with ResNet and dlib-based face recognition, achieving better performance with the latter; trained the system with one hundred face images for live recognition.
- Built a custom residual neural network with Keras for speaker recognition, achieving 96% accuracy.
- Integrated a server-client architecture using Google Cloud for accelerated processing and implemented speech recognition and TTS for user interaction.

## Key Features

- Real-time face detection and recognition
- Speaker recognition for enhanced security
- Natural language processing with ChatGPT integration
- Text-to-speech and speech-to-text capabilities
- Cloud-based processing for improved performance

## Technical Stack

- Raspberry Pi 4
- Python
- TensorFlow/Keras
- OpenCV
- dlib
- Google Cloud Services
- OpenAI API
- PyAudio
- gTTS

## Project Advisor
Prof. Deming Chen, UIUC 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/projects/raspi_iot/ras_iot.mp4" 
                              class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Demo of our ECE479 Final Porject -- "IoT Private Chatbot" (Right click on the cover above to view the video)
</div> 