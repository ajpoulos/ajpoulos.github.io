---
layout: page
permalink: /publications/
title: Publications
description: I try to keep this publication list up to date. You can also get updates by following me on <a href="https://scholar.google.com/citations?user=obdR6FoAAAAJ&hl" target="_blank">Google Scholar</a> and <a href="https://www.researchgate.net/profile/Alan-Poulos" target="_blank">ResearchGate</a>.
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017]
nav: true
---

<div class="publications">

<h1>Journal papers</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>Conference papers</h1>

{% bibliography -f conference --template bib_conference%}

</div>