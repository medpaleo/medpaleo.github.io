---
layout: single
title: People
permalink: /people/
---

{% for member in site.members %}
  <h2>
    <a href="{{ member.url }}">
      {{ member.name }} - {{ member.position }}
    </a>
  </h2>
  <p>{{ member.content | markdownify }}</p>
{% endfor %}
