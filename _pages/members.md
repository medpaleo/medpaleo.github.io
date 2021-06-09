---
title: Members
permalink: /members/
collection: members
---


<div class="grid__wrapper">
  {% for post in site.posts limit:4 %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

<div class="grid__wrapper">
  {% for member in site.members %}

  {% include archive-single.html type="grid" %}

<!--  {% capture avatar_image %} ![{{ member.author.name }}]({{member.author.avatar}}) {% endcapture %}

    {{ avatar_image | markdownify }}
    <h3>
      <a href="{{ member.url }}"> {{ member.author.name }}</a>
    </h3>
    {{ member.affiliation }} - {{ member.country }}
-->
</div>
{% endfor %}
