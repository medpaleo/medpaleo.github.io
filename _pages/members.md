---
title: Members
permalink: /members/
collection: members
---

{% for member in site.members %}

<div>
  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}){: .align-right} {% endcapture %}

  {{ avatar_image | markdownify }}
  <div>
    <h2>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h2>
    {{ member.affiliation }} - {{ member.country }}
  </div>
</div>
{% endfor %}
