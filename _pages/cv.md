---
layout: cv
permalink: /cv/
title: cv
nav: true
nav_order: 5
cv_pdf: CV-Yanghonghui Chen.pdf
description: My curriculum vitae.
toc:
  sidebar: left
---

{% assign cv = site.data.cv %}

<div class="cv">
  {% for entry in cv %}
    <div class="card mt-3 p-3">
      <h3 class="card-title font-weight-medium">{{ entry.title }}</h3>
      <div>
      {% if entry.type == "list" %}
        {% include cv/list.liquid %}
      {% elsif entry.type == "map" %}
        {% include cv/map.liquid %}
      {% elsif entry.type == "nested_list" %}
        {% include cv/nested_list.liquid %}
      {% elsif entry.type == "time_table" %}
        {% include cv/time_table.liquid data=entry %}
      {% elsif entry.type == "list_groups" %}
        {% include cv/list_groups.liquid %}
      {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
