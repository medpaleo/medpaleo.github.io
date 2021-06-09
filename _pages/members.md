---
layout: collection
title: Members
permalink: /members/
collection: members
---

{% for member in site.members %}

<div>
  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}) {% endcapture %}

  <div>
    {{ avatar_image | markdownify }}
    <h3>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h3>
    {{ member.affiliation }} - {{ member.country }}
  </div>
</div>
{% endfor %}
