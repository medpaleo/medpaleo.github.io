---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}
  {% include figure image_path="{{ member.author.avatar }}" alt="{{ member.author.name }}" %}
  <img src="{{ member.author.avatar }}" alt="{{ member.author.name }}"  height=50 width=50>
  <h2>
    <a href="{{ member.url }}">
      {{ member.author.name }}
    </a>
  </h2>
  <p>{{ member.affiliation | markdownify }} ( {{ member.country }} )</p>
{% endfor %}
