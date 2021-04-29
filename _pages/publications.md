---
layout: page
permalink: /publications/
title: publications
description: For a full list of publications, please see <b><a href="https://scholar.google.com/citations?user=vLgjEhQAAAAJ&hl=en&oi=ao">Google Scholar</a></b>.
years: [2021, 2020, 2018, 2017]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
