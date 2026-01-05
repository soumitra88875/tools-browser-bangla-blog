---
layout: default
---

<ul class="post-list">
{% for post in paginator.posts %}
  <li style="display:flex;align-items:center;margin-bottom:15px;">

    {% if post.thumbnail %}
      <img src="{{ post.thumbnail }}">
    {% endif %}

    <div>
      <a href="{{ post.url | relative_url }}">
        <b>{{ post.title }}</b>
      </a><br>

      <small style="color:#777;">
        {% assign now = site.time | date: "%s" %}
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

<!-- 🔽 Pagination START -->
<div style="text-align:center;margin:30px 0;">

  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">« Prev</a>
  {% endif %}

  {% for page in (1..paginator.total_pages) %}
    {% if page == paginator.page %}
      <strong style="margin:0 6px;">{{ page }}</strong>
    {% else %}
      <a href="{{ site.baseurl }}/page{{ page }}/" style="margin:0 6px;">
        {{ page }}
      </a>
    {% endif %}
  {% endfor %}

  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">Next »</a>
  {% endif %}

</div>
<!-- 🔼 Pagination END -->
