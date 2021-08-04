---
layout: page
permalink: /publicacoes/
title: Publicações
description: Minhas publicações em ordem cronológica reversa.
years: [2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
