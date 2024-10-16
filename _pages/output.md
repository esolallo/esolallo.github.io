---
layout: page
permalink: /output/
title: Output
ord: 30
description:

years: [2022, 2021]
nav: true
---

<!-- _pages/publications.md

### <b>Papers</b>
***
### <b>Presentations</b>
***
scholar jekyll plugin
https://www.amirasiaee.com/dailyreport/jekyll-scholar/
https://github.com/inukshuk/jekyll-scholar
-->


<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:15px;padding-bottom:10px;">Publications:</h1>
<div class="publications">
  {% bibliography -f pubs %}
</div>

<br>
<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:15px;padding-bottom:10px;">Conference proceedings:</h1>
<div class="publications">
  {% bibliography -f proceedings %}
</div>

<br>
<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:15px;padding-bottom:10px;">Conference talks:</h1>
<div class="publications">
  {% bibliography -f talks %}
</div>

<br>
<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:15px;padding-bottom:10px;">Poster presentations:</h1>
<div class="publications">
  {% bibliography -f posters %}
</div>

<br>
<h1 style="text-align:left;font-size:20px;font-weight:500;padding-top:15px;padding-bottom:10px;">Thesis:</h1>
<div class="publications">
  {% bibliography -f unpublished %}
</div>
