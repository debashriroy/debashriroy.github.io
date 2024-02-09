---
layout: page
permalink: /patents/
title: patents
description: publications by categories in reversed chronological order.
years: [2023, 2022, 2020]
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>
