---
layout: page
permalink: /publications/
title: publications
description: For the most updated and exhaustive list, check my CV  – https://bit.ly/vishesh-cv-doc
# years: [2020,2019,2018,2017,2016,2015,2014,2013, 1956, 1950, 1935, 1905]
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
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
