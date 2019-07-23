---
layout: page
title: Cours
permalink: /cours/
---

<ul>
{% assign courses = site.cours | sort: 'order' %}
{% for cours in courses %}
  {{cours.path}}
  <li {% if page.url == cours.url %} class="active"{% endif %}>
    <a href="{{ cours.url }}">{{ cours.title }}</a>
  </li>
{% endfor %}
</ul>


