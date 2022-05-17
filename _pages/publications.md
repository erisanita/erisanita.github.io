---
layout: page
permalink: /publications/
title: Publications
description: List of publications.
years: [2021, 2019, 2018, 2016, 2014]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
