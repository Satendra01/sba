---
title: "News"
layout: textlay
excerpt: "Rastriya avishkar abhiyan at IIT indore."
sitemap: false
permalink: /news.html
---



{% for article in site.data.news %}
<div style="
  border-radius: 25px;
  border: 2px solid #73AD21;
  padding: 20px;
  color:DodgerBlue;
  -webkit-box-shadow: -5px -7px 5px 2px rgba(222,175,222,1);
  -moz-box-shadow: -5px -7px 5px 2px rgba(222,175,222,1);
  box-shadow: -5px -7px 5px 2px rgba(222,175,222,1);

">
<p style="color:Tomato">{{ article.date }} </p>
<p>{{ article.headline }}</p>
</div>

{% endfor %}
