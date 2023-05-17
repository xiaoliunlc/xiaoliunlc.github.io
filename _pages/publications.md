---
layout: page
permalink: /publications/
rank: 2 # for sorting
title: Publications
description: >
  <p>An up-to-date list is available on <a href="https://scholar.google.com/citations?user=cn1k7gYAAAAJ">Google Scholar</a>.</p>
  <p>* denotes equal contribution.</p>
years: [2023, 2022, 2021, 2020, 2019, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
