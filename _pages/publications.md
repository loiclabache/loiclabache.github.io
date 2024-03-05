---
layout: page
permalink: /publications/
title: publications
description: Electronic versions of papers are provided as a professional courtesy to ensure timely dissemination of academic work for individual, noncommercial purposes. Copyright resides with the respective copyright holders, as stated within each paper. These files may not be reposted without permission.
years: [2024, 2023, 2022, 2021, 2020, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
