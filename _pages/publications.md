---
layout: page
permalink: /publications/
title: publications
order: 3
description: Kaan Akşit's scholarly publications are listed in this webpage.
years: [2022, 2021, 2020, 2019, 2018, 2017, 2015, 2014, 2013, 2012, 2011, 2010]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
