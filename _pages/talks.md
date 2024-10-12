---
layout: page
permalink: /talks/
title: talks
description: Materials for courses you taught. Replace this text with your description.
years: [2024, 2023, 2022, 2021, 2020, 2019]
nav: true
nav_order: 2
---

<!-- _pages/talks.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{%- for y in page.years %}

  <h2 class="year">{{y}}</h2>
  {% bibliography -f talks -q @*[year={{y}}]* %}
{% endfor %}

</div>
