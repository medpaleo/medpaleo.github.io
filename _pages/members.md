---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}
  <h2>
    <a href="{{ member.url }}">
      {{ member.author.name }} - {{ member.position }}
    </a>
  </h2>
  <p>{{ member.content | markdownify }}</p>
{% endfor %}
