---
title: "Blog posts"
layout: "base.njk"
---

## Some great posts

<ul>
{% for post in collections.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.data.title }}</a>
  </li>
{% endfor %}
</ul>
