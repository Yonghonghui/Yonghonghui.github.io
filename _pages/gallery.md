---
layout: page
title: Gallery
permalink: /gallery/
description: My photo collections
nav: true          # 在导航栏显示
nav_order: 6       # 导航栏显示顺序
---

<div class="gallery-container">
  {% for image in site.data.gallery %}
    <div class="gallery-item">
      <a href="{{ image.full }}" data-fancybox="gallery" data-caption="{{ image.caption }}">
        <img src="{{ image.thumb }}" alt="{{ image.caption }}">
      </a>
      <p class="caption">{{ image.caption }}</p>
    </div>
  {% endfor %}
</div> 