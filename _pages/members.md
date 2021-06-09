---
layout: single
title: Members
permalink: /members/
---

{% for member in site.members %}

  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}){: .align-left} {% endcapture %}

  {{ avatar_image | markdownify }}
  <h2>
    <a href="{{ member.url }}"> {{ member.author.name }}</a>
  </h2>
  {% include members_avatar.html max-width="100px" file=avatar_file alt=avatar_alt %} {{ member.affiliation }} - {{ member.country }}
{% endfor %}
