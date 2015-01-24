---
layout: page
---

{% include JB/setup %}

<div style="float:right">
  <a href="/assets/focos.jpg"><img alt='Fotógrafo: Pablo Carden' src='/assets/focos.jpg' height='350' /></a>
</div>

---

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

---

## “Relatos de distintos viajes”

[Relatos de viajes en bicicleta y de mochilero.](/assets/Relatos_de_distintos_viajes.pdf)

---

<br style="clear:both">
