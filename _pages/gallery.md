---
layout: page
title: Gallery
permalink: /gallery/
description: My photo collection
nav: true
nav_order: 6
---

<div class="gallery-container">
  {% for image in site.data.gallery %}
    <div class="gallery-item">
      <a href="{{ site.baseurl }}{{ image.full }}" data-fancybox="gallery" data-caption="{{ image.caption }}">
        <img src="{{ site.baseurl }}{{ image.full }}" alt="{{ image.caption }}">
      </a>
      <p class="caption">{{ image.caption }}</p>
    </div>
  {% endfor %}
</div> 