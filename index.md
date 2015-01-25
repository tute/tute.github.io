---
layout: page
---

{% include JB/setup %}

## Hoy soy

“Hoy soy” es un conjunto de cartas que fui escribiendo en distintos momentos de
mi vida. Una tarde escribí en casa el siguiente texto por ejemplo, que llamé
“Limpieza” y dio título al libro:

> Hoy limpié la casa de papeles viejos. Cartas, notas de retiros espirituales,
recuerdos varios, proyectos, emprendimientos, ideas para hacer. Hacía tiempo no
los revolvía, y por el polvo que juntaron los entendí innecesarios. Todos se
enfocaban en el futuro, eran la esperanza de llegar a hacer o a ser algo que mi
mente imaginaba.
>
> Ya no me sirven.
>
> Hoy soy.

“Hoy soy” contiene una serie de relatos cortos que divierten y hacen pensar.

[Aquí disponible para comprar](https://gumroad.com/l/hoysoy).

<a href="https://gumroad.com/l/hoysoy">
  <img alt='Fotógrafo: Pablo Carden' src='/assets/focos.jpg' height='350' />
</a>

---

## Blog posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

---

## Relatos de distintos viajes

[Relatos de viajes en bicicleta y de mochilero.](/assets/Relatos_de_distintos_viajes.pdf)

<br style="clear:both">
