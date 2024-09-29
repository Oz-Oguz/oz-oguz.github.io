---
layout: page
permalink: /publications/
title: publications
description: <b>Under Construction!!</b> - Also see <a href="https://scholar.google.com/citations?hl=en&user=0tWX-EMAAAAJ">Google Scholar</a>
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2015, 2012, 2010]
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
