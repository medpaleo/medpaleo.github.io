---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}
  <img src="{{ member.author.avatar }}" alt="{{ member.author.name }}"  height=50 width=50>
  <h2>
    <a href="{{ member.url }}"> {{ member.author.name }} </a>
  </h2>
  <p>{{ member.affiliation }} - {{ member.country }}</p>
{% endfor %}
