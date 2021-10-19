---
layout: page
permalink: /publications/
title: publications
years: [2021,2020,2017,2016,2014,2013,2009]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

{% mermaid %}
sequenceDiagram
    participant John
    participant Alice
    Alice->>John: Hello John, how are you?
    John-->>Alice: Great!
{% endmermaid %}