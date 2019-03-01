---
layout: default
title: Blog
---
<h1>Blog</h1>
<br/>
<ul>
  {% for post in site.posts %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.date || date_to_string }}</p>
      <p>{{ post.excerpt | strip_html | strip_newlines | truncate: 156}}</p>
  {% endfor %}
</ul>