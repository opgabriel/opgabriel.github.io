---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
years: [2022, 2021, 2020, 2018]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

<h1> master thesis </h1>
{% bibliography -f {{ site.scholar.theses }} -q @*[type=master]* %}

</div>

<!-- _pages/publications.md -->
<div class="publications">

<h1>conference & journal articles</h1>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>