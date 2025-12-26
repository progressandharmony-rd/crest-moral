---
layout: page
title: News
permalink: /news/
---

{% for post in site.posts %}
<div class="card">
  <div class="meta">{{ post.date | date: "%Y-%m-%d" }}</div>
  <div><a href="{{ post.url }}">{{ post.title }}</a></div>
  {% if post.excerpt %}
  <div class="meta">{{ post.excerpt | strip_html | truncate: 140 }}</div>
  {% endif %}
</div>
{% endfor %}
