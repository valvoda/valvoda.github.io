---
layout: page
permalink: /publications/
title: publications
description: For a full list of publications, please see <a href="https://scholar.google.com/citations?user=vLgjEhQAAAAJ&hl=en&oi=ao">Google Scholar</a>
years: [2018, 2019, 2020, 2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
