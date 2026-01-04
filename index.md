---
layout: default 
---
<ul class="post-list">
{% for post in site.posts %}
  <li style="display:flex;align-items:center;margin-bottom:15px;">

    {% if post.thumbnail %}
      <img src="{{ post.thumbnail }}" 
           style="width:100px;height:100px;object-fit:cover;border-radius:6px;margin-right:10px;">
    {% endif %}

    <div>
      <a href="{{ post.url }}"><b>{{ post.title }}</b></a><br>

      <small style="color:#777;">
        {% assign now = "now" | date: "%s" %}
        {% assign post_time = post.date | date: "%s" %}
        {% assign diff = now | minus: post_time %}

        {% if diff < 60 %}
          {{ diff }} sec ago
        {% elsif diff < 3600 %}
          {{ diff | divided_by: 60 }} min ago
        {% elsif diff < 86400 %}
          {{ diff | divided_by: 3600 }} hours ago
        {% elsif diff < 2592000 %}
          {{ diff | divided_by: 86400 }} days ago
        {% elsif diff < 31536000 %}
          {{ diff | divided_by: 2592000 }} months ago
        {% else %}
          {{ diff | divided_by: 31536000 }} years ago
        {% endif %}
      </small>
    </div>

  </li>
{% endfor %}
</ul>
