---
layout: default
title: "Posts"
---

# Blog Posts

{% for post in site.posts %}
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt }}</p>
  <hr>
{% endfor %}
