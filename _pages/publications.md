---
layout: page
permalink: /publications/
title: Publications
description: 
paper_years: [2022, 2021, 2020]
demo_years: [2021,2020]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">
<h3>FULL PAPER</h3>
{%- for y in page.paper_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
<div class="publications">
<h3>DEMO/EA</h3>
{%- for y in page.demo_years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f demos -q @*[year={{y}}]* %}
{% endfor %}

</div>