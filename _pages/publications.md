---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2024,2023,2022,2021]
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->


<div class="publications">

<h1>Preprints</h1>

{% bibliography -f preprints %}

<h1>Journal Articles</h1>

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

<h1>Manuscripts</h1>

{% bibliography -f manuscripts %}
  
<h1>Conference</h1>

{% bibliography -f conference %}

</div>
