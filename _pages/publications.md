---
layout: page
permalink: /publications/
title: Publications
description: Publications by year. For the most up-to-date list, please refer to my Google Scholar.
years: [2022, 2021, 2020]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
