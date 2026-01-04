---
layout: home
title: Home
---

## 📰 সর্বশেষ পোস্টসমূহ

<ul class="post-list">
{% for post in site.posts %}
  <li style="display:flex;align-items:center;margin-bottom:15px;">
    {% if post.thumbnail %}
      <img src="{{ post.thumbnail }}" style="width:80px;height:60px;object-fit:cover;border-radius:6px;margin-right:10px;">
    {% endif %}
    <a href="{{ post.url }}"><b>{{ post.title }}</b></a>
  </li>
{% endfor %}
</ul>
