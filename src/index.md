---
title: "Hello World"
layout: "base.njk"
templateEngineOverride: njk, md
---

This is a homepage.

## Random post

{% for post in collections.posts | randomPost %}
<a href="{{ post.url }}">{{ post.data.title }}</a>
{% endfor %}

## Mock articles

<ul>
{% for article in collections.articles %}
<li><a href="{{ article.url }}">{{ article.data.title }}</a></li>
{% endfor %}
</ul>
