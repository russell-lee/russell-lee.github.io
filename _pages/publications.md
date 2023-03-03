---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
<h1>conference &amp; journal articles</h1>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


<h1>preprints</h1>

{% bibliography -f preprints %}
</div>
