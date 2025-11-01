---
layout: page
permalink: /media/
title: media
description: A number of my research projects have attracted coverage from major media outlets. Where I am aware of the coverage, I have collected the links here. 
nav: true
nav_order: 5
horizontal: false
---

<!-- pages/media.md -->
<div class="media">
  {%- assign sorted_media = site.media | sort: "importance" -%}
  <!-- Generate cards for each paper -->
  <div class="grid">
    {%- for media in sorted_media -%}
      {% include media.html media=media %}
    {%- endfor %}
  </div>
</div>
