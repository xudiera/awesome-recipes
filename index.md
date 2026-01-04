---
layout: default
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<ul>
  {% for tag in site.tags %}
    <li>{{ tag[0] }} ({{ tag[1].size }})</li>
  {% endfor %}
</ul>
