---
layout: default
---
<h1>Blog</h1>
<p>Below are a list of all the blog posts I've ever written. Enjoy!</p>
<br/>
<ul>
  {% for post in site.posts %}
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
  {% endfor %}
</ul>