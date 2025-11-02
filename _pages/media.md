---
layout: page
permalink: /press/
title: press
description: A number of my research projects have attracted press coverage. Where I am aware of the coverage, I have collected the links here. If you are interested in writing about one of my papers, I'd be happy to hear from you!
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
