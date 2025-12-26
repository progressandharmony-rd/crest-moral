---
layout: home
title: Home
---

<!--
# Project MORAL

**身体が考えるロボット基盤モデル：MORAL**

---
-->

## News
{% for post in site.posts limit:5 %}
<div class="card">
  <div class="meta">{{ post.date | date: "%Y-%m-%d" }}</div>
  <div><a href="{{ post.url }}">{{ post.title }}</a></div>
</div>
{% endfor %}

[View All News →](/news/)
