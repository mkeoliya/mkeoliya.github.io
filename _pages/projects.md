---
layout: page
permalink: /projects/
title: projects
description: things that i've worked on
years: [2022]
nav: true
nav_order: 2
---
<!-- _pages/projects.md -->
<div class="publications">
<h2>papers</h2>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
