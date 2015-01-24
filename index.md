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

## Textos míos

[“En el día de hoy”, cuentos, cartas, reflexiones.](/assets/libro/Cartas.pdf)

---

<br style="clear:both">
