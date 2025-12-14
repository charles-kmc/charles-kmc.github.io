---
layout: page
permalink: /publications/
title: publications
description:
years: [2024, 2025]
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{%- assign sorted_years = page.years | sort: 'to_integer' | reverse -%}
{%- for y in sorted_years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -f papers -q @*[year={{ y }}]* %}
{%- endfor %}

</div>
