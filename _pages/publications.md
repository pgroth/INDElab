---
layout: about
permalink: /publications/
title: publications
description: Selected recent publications from Paul as we get started . Generated by jekyll-scholar.
years: [2018,2017,2016]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}