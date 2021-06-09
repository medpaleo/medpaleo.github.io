---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}

  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}){: .align-left} {% endcapture %}

  {{ avatar_image | markdownify }}
  <div>
    <h2>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h2>
    {{ member.affiliation }} - {{ member.country }}
  </div>
{% endfor %}
