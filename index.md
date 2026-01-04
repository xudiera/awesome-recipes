---
layout: default
---

<h2>Pages</h2>
<ul>
  {% for page in site.pages %}
    {% if page.title %}
      <li>
        <a href="{{ page.url | relative_url }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>
<h2>Recipes</h2>
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