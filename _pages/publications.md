---
layout: page2
permalink: /publications/
title: Papers
years: [Working Paper, Submitted, 2021,2019, 2017,2016,2014,2013,2009]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

