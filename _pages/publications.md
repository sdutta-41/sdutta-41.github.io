---
layout: page
permalink: /publications/
title: publications
# description: publications by categories in reversed chronological order. generated by jekyll-scholar.
years: [1956, 1950, 1935, 1905]
nav: false
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>