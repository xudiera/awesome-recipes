---
layout: default
---

<h1>Recipes</h1>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
<h2>Tags</h2>
<ul>
  {% assign tags_sorted = site.tags | sort %}
  {% for tag in tags_sorted %}
    <li>
      <a href="{{ '/tags.html' | relative_url }}#{{ tag[0] }}">{{ tag[0] }} ({{ tag[1].size }})</a>
    </li>
  {% endfor %}
</ul>
