---
layout: default
title: "Notes — fyiKamran"
description: "Quick thoughts, links, and commentary."
---
{% assign microposts = site.microposts | sort: 'date' | reverse %}
{% for post in microposts %}
<article class="micro-post">
  <time>{{ post.date | date: "%d %b %Y" }}</time>
  {% if post.type == "link" %}
    <a href="{{ post.url }}" class="micro-link">{{ post.url }}</a>
  {% endif %}
  {{ post.content }}
</article>
{% endfor %}
