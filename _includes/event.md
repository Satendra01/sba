



{% for article in site.data.events %}
<div style="
  border-radius: 25px;
  border: 2px solid #73AD21;
  padding: 20px;
  color:Tomato;
  -webkit-box-shadow: inset -5px -7px 5px 2px rgba(70,100,219,1);
-moz-box-shadow: inset -5px -7px 5px 2px rgba(70,100,219,1);
box-shadow: inset -5px -7px 5px 2px rgba(70,100,219,1);
">
<p>
<em>{{ article.headline }}</em></p>
</div>

{% endfor %}
