---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2025, 2024, 2023, 2022, 2021, 2020, 2018]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<h1> phd & master's theses </h1>
{% bibliography -f {{ site.scholar.theses }} %}

</div>

<!-- _pages/publications.md -->
<div class="publications">

<h1>conference & journal articles</h1>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>