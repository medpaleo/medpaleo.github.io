---
title: Members
layout: collection
permalink: /members/
collection: members
entries_layout: grid
class: wide
---

<div class="grid__wrapper">
  {% for member in site.members %}

  {% include member.html type="grid" %}

<!--  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}) {% endcapture %}

    {{ avatar_image | markdownify }}
    <h3>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h3>
    {{ member.affiliation }} - {{ member.country }}
-->
</div>
{% endfor %}
