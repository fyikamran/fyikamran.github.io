---
layout: default
title: "Micro Blog — fyiKamran"
description: "Quick thoughts, links, and commentary."
---

<h1>Kamran</h1>
<p style="color: var(--text-muted); margin-top: -0.75rem;">Short posts, links, and notes.</p>

{% assign microposts = site.microposts | sort: 'date' | reverse %}
{% for post in microposts %}
<article style="padding: 1.25rem 0; border-bottom: 1px solid var(--text-muted); opacity: 0.9;">
  <time style="display: block; font-size: 0.8rem; color: var(--text-muted); margin-bottom: 0.5rem;">{{ post.date | date: "%d %b %Y" }}</time>
  {% if post.type == "link" %}
    <a href="{{ post.url }}" class="micro-link" style="font-size: 0.9rem;">{{ post.url }}</a>
  {% endif %}
  <div style="font-size: 0.95rem; line-height: 1.6;">{{ post.content }}</div>
</article>
{% endfor %}

