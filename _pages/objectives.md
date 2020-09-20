---
title: "EBSB @ IITi - Objectives"
layout: gridlay
excerpt: "EBSB @IITi -- Objectives."
sitemap: false
permalink: /objectives/
---


# <ins style="font-size: 30px; font-weight:600">Objectives & Themes for Interaction</ins>
Jump to [Objectives](#objectives), [Critical Themes for Interaction](#themes)

## <ins style="font-size: 29px;">Objectives</ins>
<br>
{% assign number_printed = 0 %}
{% for publi in site.data.objlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-12 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

<hr>

# <ins style="font-size: 30px; font-weight:600">Themes</ins>
Jump back to [Objectives](#objectives)
## <ins style="font-size: 29px;">Critical Themes for Interaction</ins>
<br>
<div class="col-sm-12 clearfix">
 <div class="well">
{% for publi in site.data.objlist %}
{% if publi.highlight == 0 %}
  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>
{% endif %}
{% endfor %}
</div>
</div>
