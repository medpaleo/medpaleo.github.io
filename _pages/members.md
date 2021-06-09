---
title: Members
layout: collection
permalink: /members/
collection: members
entries_layout: grid
class: wide
---

{% for member in site.members %}

  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}) {% endcapture %}

    {{ avatar_image | markdownify }}
    <h3>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h3>
    {{ member.affiliation }} - {{ member.country }}

{% endfor %}
