---
layout: page
permalink: /talks/
title: talks
description:
years: [2024,2023,2022]
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
