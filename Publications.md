---
layout: page
title: Publications
permalink: /publications/
years: [2024,2019]
---

{% for y in page.years %}
  <h3  id="{{y}}" class="pubyear">{{y}}</h3>
  {% bibliography -q @*[year={{y}}]* %}
{% endfor %}
