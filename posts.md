---
layout: default
title: "Posts"
---

# Blog Posts

<div style="text-align: center; margin-top; 50px;">
  <h1 style="font-size: 2.5em;">Blog Ports</h1>

{% for post in site.posts %}
  <div style="margin-top: 20px; text-align: left;">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y" }}</p>
  <p>{{ post.excerpt }}</p>
  <hr>
  </div>
{% endfor %}
</div>  
