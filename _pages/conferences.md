---
layout: page
permalink: /conferences/
title: conferences
description: publications by categories in reversed chronological order.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2014, 2013]
<!-- nav: true
nav_order: 1 -->
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f conferences -q @*[year={{y}}]* %}
{% endfor %}

</div>