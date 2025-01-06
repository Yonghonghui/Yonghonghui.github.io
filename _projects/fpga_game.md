---
layout: page
title: FPGA Multiplayer Game
description: Implemented a multiplayer action game 'Crazy Arcade' on FPGA using SystemVerilog
# img: assets/img/projects/fpga_game/thumbnail.jpg
importance: 1
category: Hardware & Systems
github: https://github.com/Yonghonghui/ECE-385---Digital-Systems-Laboratory
---

## Overview

Developed a complete multiplayer action game "Crazy Arcade" on FPGA, integrating MicroBlaze CPU for game logic and keyboard input processing, with real-time graphics and sound capabilities.

<!-- ## Links

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  <div class="repo p-2">
    <h5 class="font-weight-bold text">GitHub Repository</h5>
    <a href="https://github.com/YourUsername/fpga-game" target="_blank">
      <i class="fab fa-github"></i> FPGA Crazy Arcade Game
    </a>
  </div>
  
  <div class="repo p-2">
    <h5 class="font-weight-bold text">Documentation</h5>
    <a href="path_to_documentation" target="_blank">
      <i class="fas fa-book"></i> Technical Docs
    </a>
  </div>
  
  <div class="repo p-2">
    <h5 class="font-weight-bold text">Live Demo</h5>
    <a href="demo_url" target="_blank">
      <i class="fas fa-play"></i> Try it out
    </a>
  </div>
</div> -->

## Project Demo

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/5.jpg" title="Original Crazy Arcade" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The original Crazy Arcade game that inspired this FPGA implementation.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/bomb.jpg" title="Gameplay Screenshot" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Screenshot of the Crazy Arcade game running on FPGA, showing the multiplayer interface and bomb mechanics.
</div>

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/system_architecture.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/4.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: System architecture diagram showing the integration of various components. Right: Physical FPGA setup with VGA display and keyboard input.
</div>

<div class="row">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/Kun.jpg" title="Player 1 Explosion" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/doll.jpg" title="Player 2 Explosion" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/projects/fpga_game/gameover.jpg" title="Game Over Screen" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Game screen showcase: Left image shows Player 1 being hit by an explosion, middle image shows Player 2 being hit by an explosion, and right image displays the game over screen.
</div>

## Technical Details

- Implemented core game components:
  - MicroBlaze CPU integration for game logic
  - Real-time keyboard input processing
  - VGA display controller
  - PWM-based sound generation
- Developed SystemVerilog modules for:
  - Player movement mechanics
  - Bomb placement and explosion
  - Life count management
  - Game state control
  - System bus communication

## Key Features

- Real-time multiplayer gameplay
- Hardware-accelerated graphics
- Interactive sound system
- Responsive controls
- State-based game logic
- System bus integration

## Technical Stack

- SystemVerilog
- FPGA Development
- MicroBlaze CPU
- VGA Graphics
- PWM Audio
- System-on-Chip Design
- Hardware Description Language
- Real-time Systems

## Project Advisor
Prof. Zuofu Cheng, UIUC 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/projects/fpga_game/game.mp4" 
                              class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Demo of our ECE385 Final Porject -- "Crazy Arcade"
</div> 