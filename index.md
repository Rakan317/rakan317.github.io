---
layout: default
title: Home
---

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </article>
{% endfor %}
