---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->
<div class="publications">
<p><a href='https://scholar.google.com/citations?user=tnOczoAAAAAJ&hl=en'>Here</a> is the link to my google scholar.</p>
<br />
<p>* indicates equal contribution</p>
<h3>Published</h3>
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

