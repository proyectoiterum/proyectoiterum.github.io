---
title: Recetas
layout: collection
permalink: /recetas/
---

{% for category in site.categories %}
{% if category[0] == "receta" %}
{% for post in category[1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
{% endif %}
{% endfor %}
