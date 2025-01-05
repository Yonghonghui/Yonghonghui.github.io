---
layout: page
title: Gallery
permalink: /gallery/
description: My photo collection
nav: true
nav_order: 6
---

<style>
.gallery-container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 20px;
  padding: 20px;
}

.gallery-item {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}

.gallery-item:hover {
  transform: translateY(-5px);
}

.gallery-item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  display: block;
}

.caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0,0,0,0.7);
  color: white;
  padding: 10px;
  margin: 0;
  font-size: 0.9em;
  text-align: center;
}
</style>

<div class="gallery-container">
  {% for image in site.data.gallery %}
    <div class="gallery-item">
      <img src="{{ image.full }}" alt="{{ image.caption }}">
      <p class="caption">{{ image.caption }}</p>
    </div>
  {% endfor %}
</div> 