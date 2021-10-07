---
layout: page
permalink: /publications/
title: Publications
description: Asterisks (*) denote equal contribution. Order of authors determined via conflip.
years: [2021,2020,2019,2018]
nav: true
---

An up-to-date list can also be found on my Google Scholar profile [here](https://scholar.google.com/citations?user=iBuxBEUAAAAJ).

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
