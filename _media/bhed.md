---
layout: page
title: "Indian-BhED: A Dataset for Measuring India-Centric Biases in Large Language Models"
#img: assets/img/OII_small_blue_logo.jpg
permalink: /media/bhed/
# list of name/url pairs
links:
  - publisher: "MIT Technology Review"
    name: "OpenAI is huge in India. Its models are steeped in caste bias."
    url: "https://www.technologyreview.com/2025/10/01/1124621/openai-india-caste-bias/"
    date: "Oct. 1, 2025"
importance: 4
related_publications: khandelwalIndianBhEDDatasetMeasuring2024
---

{%- if page.related_publications != null and page.related_publications.size > 0 -%}
{% assign publications = page.related_publications | replace: ", ", "," | split: "," | join: "|" %}
<div class="abstract">
{% bibliography -f {{ site.scholar.bibliography }} -q @*[key^={{ publications }}]* --template {{entry.abstract}} %}
</div>
{%- endif %}