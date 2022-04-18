---
layout: page
permalink: /publications/
title: publications
description: For the most updated and exhaustive list, <a href="https://bit.ly/vishesh-cv">check my CV by clicking here!</a>
years: [2020,2019,2018,2017,2016,2015,2014,2013]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
