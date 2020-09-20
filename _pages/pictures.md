---
title: "Pictures-SBA @IITi"
layout: piclay
excerpt: "SBA@IITi -- Pictures"
permalink: /pictures/
---

<!-- # <ins style="font-size: 30px; font-weight:600">Pictures </ins>
Jump to: [IIT Indore Video](#IITIndore), [Gallery](#gallery)


## <ins style="font-size: 29px;">IIT Indore</ins>

#### IIT Indore Video [(go to website)](https://iiti.ac.in):
<iframe width="315" height="315" src="https://www.youtube.com/embed/UScf6RseI7w" frameborder="0" allowfullscreen></iframe>
<hr> -->
{% include pictures.html %}
<hr style="height: 15px;
        border: 0;
        box-shadow: inset 0 12px 12px -12px rgba(9, 84, 132);">
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
  <a href="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" target="_blank">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" /></a>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
