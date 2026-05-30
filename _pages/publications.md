---
layout: page
permalink: /publications/
title: publications
description: publications by year, project details coming soon.
years: [2026, 2025, 2024, 2023, 2022]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
