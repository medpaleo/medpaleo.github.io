---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}
  <h2>
    <img src="{{ member.author.avatar }}" alt="{{ member.author.name }}">
    <a href="{{ member.url }}">
      {{ member.author.name }}
    </a>
  </h2>
  <p>{{ member.affiliation | markdownify }} ( {{ member.country }} )</p>
{% endfor %}
