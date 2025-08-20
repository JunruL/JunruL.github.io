---
layout: page
permalink: /publications/
title: Publication
years: [2022, 2024, 2025]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- assign reversed_years = page.years | sort | reverse %}
{%- for y in reversed_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
