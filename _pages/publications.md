---
layout: page
permalink: /publications/
title: publications
description: For a full list of publications, please see [Google Scholar](https://scholar.google.com/citations?user=vLgjEhQAAAAJ&hl=en&oi=ao){:target="\_blank"}.
years: [2021, 2020, 2018, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
